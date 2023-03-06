# Documentation


Bring Your Own Key (BYOK) is a feature that allows SFMC (Salesforce Marketing Cloud) users to manage their own encryption keys for encryption at rest. With BYOK, users can choose to use their own encryption keys instead of the default encryption keys generated and managed by SFMC. This provides users with greater control over the security and protection of their data.

Implementation Steps:

    Generate an encryption key: Users can generate an encryption key using a third-party key management system or a hardware security module (HSM).

    Import the encryption key to SFMC: Once the encryption key is generated, users can import the key to SFMC by using the Key Management Interoperability Protocol (KMIP). KMIP is a protocol that allows communication between key management systems and cryptographic devices.

    Enable BYOK: To enable BYOK, users must contact SFMC Support and provide the following information:

    The name and version of the key management system or HSM being used.
    The key provider URL and authentication credentials.
    The public certificate for the key management system.

After verifying the information, SFMC Support will enable BYOK for the account.

    Configure encryption settings: Users can configure encryption settings for individual data fields within a data extension by selecting the "Encrypt" option when creating or editing a data extension.

Limitations:

    BYOK is only available for Enterprise 2.0 and above editions of SFMC.
    Users are responsible for managing and protecting their own encryption keys. If the encryption key is lost or compromised, SFMC will not be able to access the encrypted data.
    BYOK may impact performance, especially when encrypting large amounts of data.

Best Practices:

    Use a secure key management system or HSM: The key management system or HSM used for BYOK should be secure and meet industry standards for key management and protection.
    Store encryption keys securely: Encryption keys should be stored securely to prevent unauthorized access or theft.
    Regularly rotate encryption keys: Regularly rotating encryption keys helps ensure the integrity of the encryption.

Conclusion:
BYOK is a powerful feature that provides SFMC users with greater control over the security and protection of their data. By following the implementation steps and best practices outlined in this documentation, users can ensure that their data is secure and protected from unauthorized access. However, it is important to keep in mind the limitations of BYOK and implement additional security measures as necessary.
