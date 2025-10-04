
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;
import java.util.ArrayList;

public class CustomerListSystem extends JFrame {
    private ArrayList<String[]> customers; 
    private JTextField nameField, contactField, addressField, searchField;
    private JTextArea outputArea;

    public CustomerListSystem() {
        customers = new ArrayList<>();

        // Frame setup
        setTitle("CUSTOMER RECORDS MANAGER SYSTEM");
        setSize(600, 500);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null);

        // Dark background
        JPanel mainPanel = new JPanel();
        mainPanel.setLayout(new BorderLayout());
        mainPanel.setBackground(Color.DARK_GRAY);
        add(mainPanel);

        // Input Panel (Top)
        JPanel inputPanel = new JPanel(new GridLayout(4, 2, 10, 10));
        inputPanel.setBackground(Color.DARK_GRAY);

        JLabel nameLabel = new JLabel("Name:");
        JLabel contactLabel = new JLabel("Contact No:");
        JLabel addressLabel = new JLabel("Address:");
        JLabel searchLabel = new JLabel("Search Customer:");

        // White text on labels
        nameLabel.setForeground(Color.WHITE);
        contactLabel.setForeground(Color.WHITE);
        addressLabel.setForeground(Color.WHITE);
        searchLabel.setForeground(Color.WHITE);

        nameField = new JTextField();
        contactField = new JTextField();
        addressField = new JTextField();
        searchField = new JTextField();

        JButton searchBtn = createButton("Search", Color.BLUE, Color.WHITE);

        inputPanel.add(nameLabel);
        inputPanel.add(nameField);
        inputPanel.add(contactLabel);
        inputPanel.add(contactField);
        inputPanel.add(addressLabel);
        inputPanel.add(addressField);
        inputPanel.add(searchLabel);

        // Panel for search field + button
        JPanel searchPanel = new JPanel(new BorderLayout());
        searchPanel.setBackground(Color.DARK_GRAY);
        searchPanel.add(searchField, BorderLayout.CENTER);
        searchPanel.add(searchBtn, BorderLayout.EAST);

        inputPanel.add(searchPanel);

        mainPanel.add(inputPanel, BorderLayout.NORTH);

        // Buttons Panel (Middle)
        JPanel buttonPanel = new JPanel(new FlowLayout());
        buttonPanel.setBackground(Color.DARK_GRAY);

        JButton addBtn = createButton("Add Customer", Color.CYAN, Color.BLACK);
        JButton deleteBtn = createButton("Delete Customer", Color.BLUE, Color.WHITE);
        JButton showBtn = createButton("Show All Customers", Color.WHITE, Color.BLACK);

        buttonPanel.add(addBtn);
        buttonPanel.add(deleteBtn);
        buttonPanel.add(showBtn);

        mainPanel.add(buttonPanel, BorderLayout.CENTER);

        // Output Area (Bottom)
        outputArea = new JTextArea(10, 40);
        outputArea.setEditable(false);
        outputArea.setBackground(Color.BLACK);
        outputArea.setForeground(Color.GREEN);
        JScrollPane scrollPane = new JScrollPane(outputArea);
        mainPanel.add(scrollPane, BorderLayout.SOUTH);

        // Button Actions
        addBtn.addActionListener(e -> addCustomer());
        deleteBtn.addActionListener(e -> deleteCustomer());
        searchBtn.addActionListener(e -> searchCustomer());
        showBtn.addActionListener(e -> showAllCustomers());

        setVisible(true);
    }

    // Helper method to create styled buttons
    private JButton createButton(String text, Color bg, Color fg) {
        JButton button = new JButton(text);
        button.setBackground(bg);
        button.setForeground(fg);
        button.setFocusPainted(false);
        button.setFont(new Font("Arial", Font.BOLD, 14));
        return button;
    }

    // Add customer with validation
    private void addCustomer() {
        String name = nameField.getText().trim();
        String contact = contactField.getText().trim();
        String address = addressField.getText().trim();

        if (name.isEmpty() || contact.isEmpty() || address.isEmpty()) {
            outputArea.setText("⚠ Please fill in all fields!\n");
            return;
        }

        // Contact number validation: must be numeric and 11 digits
        if (!contact.matches("\\d{11}")) {
            outputArea.setText("⚠numbers only, and must be 11 digits!\n");
            return;
        }

        customers.add(new String[]{name, contact, address});
        outputArea.setText("✅ Customer added successfully!\n");
        clearFields();
    }

    // Delete customer
    private void deleteCustomer() {
        String name = nameField.getText().trim();
        if (name.isEmpty()) {
            outputArea.setText("⚠ Enter a name to delete!\n");
            return;
        }

        boolean removed = false;
        for (int i = 0; i < customers.size(); i++) {
            if (customers.get(i)[0].equalsIgnoreCase(name)) {
                customers.remove(i);
                removed = true;
                break;
            }
        }

        if (removed) {
            outputArea.setText("🗑 Customer '" + name + "' deleted!\n");
        } else {
            outputArea.setText("❌ Customer not found!\n");
        }
        clearFields();
    }

    // Search customer
    private void searchCustomer() {
        String searchName = searchField.getText().trim();
        if (searchName.isEmpty()) {
            outputArea.setText("⚠ Enter a name to search!\n");
            return;
        }

        StringBuilder sb = new StringBuilder();
        for (String[] c : customers) {
            if (c[0].equalsIgnoreCase(searchName)) {
                sb.append("🔍 Found Customer:\n");
                sb.append("Name: ").append(c[0]).append("\n");
                sb.append("Contact: ").append(c[1]).append("\n");
                sb.append("Address: ").append(c[2]).append("\n");
            }
        }

        if (sb.length() == 0) {
            outputArea.setText("❌ No customer found with name: " + searchName + "\n");
        } else {
            outputArea.setText(sb.toString());
        }
    }

    // Show all customers
    private void showAllCustomers() {
        if (customers.isEmpty()) {
            outputArea.setText("⚠ No customers in the system.\n");
            return;
        }

        StringBuilder sb = new StringBuilder("📋 Customer List:\n");
        for (String[] c : customers) {
            sb.append("\n Name: ").append(c[0])
              .append(", \n Contact: ").append(c[1])
              .append(", \n Address:").append(c[2]).append("\n");
        }
        outputArea.setText(sb.toString());
    }

    // Clear input fields
    private void clearFields() {
        nameField.setText("");
        contactField.setText("");
        addressField.setText("");
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(CustomerListSystem::new);
    }
}

