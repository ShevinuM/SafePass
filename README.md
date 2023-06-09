# SafePass

## Project Description
SafePass is a user-friendly and secure tool designed to manage strong and unique passwords. With a focus on user privacy and data protection, this application ensures that passwords are only stored locally if the user wishes to, offering an additional layer of security by eliminating the need for server storage. Offering the user the opportunity to store in a web server if they prefer the added flexibility over the increased security storing only locally is something I am considering too.

By leveraging cryptographic algorithms, the Password Generator enables users to create passwords of varying lengths and complexity. The customizable options include uppercase and lowercase letters, numbers, and special characters, allowing users to tailor their passwords to meet their specific security requirements.

One of the project's key advantages lies in its commitment to user privacy. By exclusively storing passwords locally, it eliminates the risk associated with centralized server storage, providing users with enhanced peace of mind regarding the protection of their sensitive information.

In a world where most password storing apps rely on server storage solutions, it can be challenging to find an application that prioritizes local storage for enhanced privacy and control. That's why I developed this application, a password manager that focuses on storing your sensitive data locally, right on your device.

The Password Generator's intuitive interface makes it accessible to users of all technical backgrounds. Additionally, the ability to copy generated passwords directly to the clipboard streamlines the password integration process across various applications and platforms.

With the inclusion of a password strength indicator, users can conveniently assess the robustness of their generated passwords. This visual feedback empowers users to make informed decisions about the strength and security of their chosen passwords.

Open-source in nature, the Password Generator project encourages collaboration, feedback, and customization from the developer community, fostering continuous improvement and innovation in the realm of password security.

## Key Features
- Customizable Password Generation: Users can specify the desired length and complexity of the passwords generated. Options may include uppercase and lowercase letters, numbers, special characters, and more.
- Secure and Strong Passwords: The password generator utilizes cryptographic algorithms to generate random passwords, ensuring high security and unpredictability.
- User-Friendly Interface: The project offers an intuitive and easy-to-use interface, making it accessible to users with varying levels of technical expertise.
- Copy to Clipboard: Users can quickly copy generated passwords to their system clipboard, enabling seamless integration with other applications and platforms.
- Password Strength Indicator: The project may include a feature to visually indicate the strength of the generated password, helping users assess its robustness.
- Transfer Password Vault: Safely and securely transfer your password vault between computers using encrypted files. This feature allows you to export your password vault as an encrypted file, which can be transferred to another computer and imported securely into the password manager.
- Offline Access: Access your passwords and sensitive information even without an internet connection, ensuring seamless availability whenever you need it.

## Security Measures
- Security of the user data is the highest priority in this application. here are some of the main security measures to be implemented:
  - **Hashing and Salting:** User passwords are not stored in plaintext. They are    hashed using PBKDF2 with HmacSHA256 algorithm, which is a widely accepted secure method for password hashing. A unique salt is generated for each password, preventing rainbow table attacks.
  - **Secure Storage:** All the hashed and salted passwords are then encrypted using a key derived from the user's master password, adding an additional layer of security. Even if an attacker gets hold of the stored data, they won't be able to decrypt the passwords without the master password.
  - **Master Password Verification:** The application verifies the master password using a secure method. The master password itself is never stored. Instead, a hashed and salted version is stored. When verifying, the entered password is hashed and salted in the same way and then compared.

## Benefits
- Local Storage: Your passwords and sensitive information are securely stored on your device, giving you full control over your data.
- Enhanced Security: By generating strong and unique passwords, the application promotes better security practices, reducing the risk of unauthorized access to personal or sensitive data.
- Time-Saving: With the password generator, users no longer need to manually come up with secure passwords or rely on weak, easily guessable ones. This saves time and effort while ensuring stronger password protection.
- Versatility: The application can be used in various contexts, such as creating passwords for online accounts, Wi-Fi networks, encrypted files, or any other situation requiring secure password generation.
Open Source: The project may be open source, encouraging collaboration, feedback, and customization from the developer community.

## Current Implementations
- Serialization: The project utilizes serialization to store and retrieve data. Serialized objects are stored locally, providing a secure and efficient means of data persistence.

## Future Plans
- The project is currently under active development, and there are several exciting features and enhancements planned for the future. While the project is in the direction of making progress, it's important to note that not all features listed below have been completed or started at this stage.

## Project Structure
The Java files for this project are located in the following directory:
- `src`: This folder contains the source code of the project.
- `main/java`: Java files are located within this directory.
- `com/example/projectname/`: This represents the package structure of the project.
You can navigate to the appropriate folder to access and explore the Java files related to this project.

