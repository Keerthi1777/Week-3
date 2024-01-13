import java.util.ArrayList;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;

public class ExpenseTracker {
    private Map<String, User> users;
    private User currentUser;
    private Scanner scanner;

    public ExpenseTracker() {
        this.users = new HashMap<>();
        this.scanner = new Scanner(System.in);
    }

    public static void main(String[] args) {
        ExpenseTracker expenseTracker = new ExpenseTracker();
        expenseTracker.run();
    }

    private void run() {
        // Implement the main menu and user interaction here
        // Consider options like user registration, expense entry, listing, etc.
    }

    private class User {
        private String username;
        private String password;
        private List<Expense> expenses;

        public User(String username, String password) {
            this.username = username;
            this.password = password;
            this.expenses = new ArrayList<>();
        }

        // Implement methods for expense entry, listing, and other user-related functionalities
    }

    private class Expense {
        private String date;
        private String category;
        private double amount;

        public Expense(String date, String category, double amount) {
            this.date = date;
            this.category = category;
            this.amount = amount;
        }

        // Implement any additional methods for expense manipulation
    }
}
