#include<iostream>
#include<string>
#include<vector>
using namespace std;

// Class to store and manage individual user information
class User {
	private:
		string username, password;
	public:
		// Constructor to initialize user
		User(string name, string pass) {
			username = name;
			password = pass;
		}
		// Get username
		string getUsername() {
			return username;
		}
		// Get password
		string getPassword() {
			return password;
		}
};

// Class to manage multiple users
class UserManager {
	private:
		vector<User> users; // Vector to store user objects
	public:
		// Register a new user
		void RegiserUser() {
			string username, password;
			cout << "\t\tEnter User Name : ";
			cin >> username;
			cout << "\t\tEnter Password : ";
			cin >> password;

			User newUser(username, password);
			users.push_back(newUser);

			cout << "\t\tUser Registered Successfully ....." << endl;
		}

		// Login an existing user
		bool LoginUser(string name, string pass) {
			for (int i = 0; i < users.size(); i++) {
				if (users[i].getUsername() == name && users[i].getPassword() == pass) {
					cout << "\t\tLogin Successfully...." << endl;
					return true;
				}
			}
			cout << "\t\tInvalid User Name or Password..." << endl;
			return false;
		}

		// Display all registered users
		void showUser() {
			cout << "\t\t---Users List---" << endl;
			for (int i = 0; i < users.size(); i++) {
				cout << "\t\t" << users[i].getUsername() << endl;
			}
		}

		// Search a user by username
		void searchUser(string username) {
			for (int i = 0; i < users.size(); i++) {
				if (users[i].getUsername() == username) {
					cout << "\t\tUser Found" << endl;
				}
			}
		}

		// Delete a user by username
		void deleteUser(string username) {
			for (int i = 0; i < users.size(); i++) {
				if (users[i].getUsername() == username) {
					users.erase(users.begin() + i);
					cout << "\t\tUser Removed Successfully...." << endl;
				}
			}
		}
};

int main() {
	UserManager usermanage;

	int op;
	char choice;
	do {
		system("cls"); // Clear screen for clean UI

		// Main menu
		cout << "\n\n\t\t1. Register User " << endl;
		cout << "\t\t2. Login " << endl;
		cout << "\t\t3. Show User List " << endl;
		cout << "\t\t4. Search User " << endl;
		cout << "\t\t5. Delete User" << endl;
		cout << "\t\t6. Exit" << endl;

		cout << "\t\tEnter Your Choice : ";
		cin >> op;

		// Handle user input
		switch (op) {
			case 1: {
				usermanage.RegiserUser();
				break;
			}
			case 2: {
				string username, password;
				cout << "\t\tEnter User : ";
				cin >> username;
				cout << "\t\tEnter Password : ";
				cin >> password;
				usermanage.LoginUser(username, password);
				break;
			}
			case 3: {
				usermanage.showUser();
				break;
			}
			case 4: {
				string username;
				cout << "\t\tEnter User Name : ";
				cin >> username;
				usermanage.searchUser(username);
				break;
			}
			case 5: {
				string username;
				cout << "\t\tEnter User Name : ";
				cin >> username;
				usermanage.deleteUser(username);
				break;
			}
			case 6:
				exit(op);
		}

		cout << "\t\tDo You Want to Continue [Yes/No]? : ";
		cin >> choice;

	} while (choice == 'y' || choice == 'Y');
}
