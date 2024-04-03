import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;

public class Department {
    private int id;
    private String name;
    public Department(int id, String name) {
        this.id = id;
        this.name = name;
    }
    public int getId() {
        return id;
    }
    public String getName() {
        return name;
    }
    public static void main(String[] args) {
        String url = "jdbc:mysql://localhost:3306/departments";
        String username = "root";
        String password = "root"; 

        Department department = new Department(101, "CSE");

        try (Connection connection = DriverManager.getConnection(url, username, password)) {
            String query_stmnt= "INSERT INTO department (id, name) VALUES (" + department.getId() + ", '" + department.getName() + "')";

            try (Statement statement = connection.createStatement()) {
                int rowsAffected = statement.executeUpdate(query_stmnt);
                if (rowsAffected == 1) {
                    System.out.println("Department inserted.");
                } else {
                    System.out.println("Failed to insert.");
                }
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
