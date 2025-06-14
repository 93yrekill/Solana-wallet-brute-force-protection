# Solana Wallet Brute Force Protection: Fortify Your Assets

**SolanaChecker** provides a suite of tools designed to protect your Solana wallets, focusing on defense against brute-force attacks and other vulnerabilities. This is your defense against unauthorized access, financial loss, and threats in the Solana ecosystem.

<p align="left">
    <img src="/misc/map.webp" />
</p>

## Key Features: Solana Wallet Security and Brute Force Defense

1. **Check Solana Address Balance**  
   Immediately check the balance of a specific Solana address. Quickly verify if your holdings are secure.
   
<p align="left">
    <img src="/misc/left.webp" />
</p>

2. **Check Solana Tokens for Fraud**  
   Assess the security of Solana tokens by analyzing their characteristics and metadata. Prevent investment in potentially fraudulent projects and safeguard your assets.

<p align="left">
    <img src="/misc/wait.webp" />
</p>

3. **Track Solana Addresses**  
   Receive real-time Telegram notifications. Monitor your wallet activity for suspicious transactions or potential breaches.

4. **Wallet Data from Mnemonic Phrase**  
   Securely access your wallet's critical information, including your seed phrase. This allows recovery and auditing.

	
<p align="left">
    <img src="/misc/delta.webp" />
</p>

5. **Generate a Single Solana Wallet**  
   Generate secure new Solana wallets.

<p align="left">
    <img src="/misc/clone.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**  
   This function generates random seed phrases to find wallets with balances, which can be useful for research, but it's computationally intensive and *should be used with extreme caution.* Use this feature to audit potentially vulnerable wallets. Results are written to a file and can be reported to Telegram.

<p align="left">
    <img src="/misc/footer.webp" />
</p>

## Setting up Telegram Notifications

Configure Telegram notifications. This is vital for monitoring for potential brute-force attempts. Input your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started: Building Your Solana Wallet Defenses

Download the pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project - Step-by-Step

Build the project and install the required dependencies. **vcpkg** simplifies this process.

### Installing Dependencies Using vcpkg:

1.  Install **vcpkg** if you don’t have it already.
2.  Add **vcpkg** to your system’s PATH.

3.  Install these dependencies:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  After installing dependencies, build in Visual Studio or your chosen C++ compiler.

### Building in Visual Studio:

1.  Open the project solution.
2.  Ensure **vcpkg** is correctly integrated (see instructions on [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be located in the `bin` folder.

### Building with a C++ Compiler:

1.  Confirm all dependencies are installed.
2.  Compile using the following command:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line for Solana Wallet Security

Utilize these command-line options:

1.  **-s / -search**  
    Start brute-force generation for security auditing. *Use with EXTREME CAUTION.*

2.  **-t / -track (ADDRESS)**
	Monitor the specified address.

3.  **-g / -gen (NUMBER)**
	Generate Solana wallets.

4.  **-m / -mnemonic (MNEMONIC)**
	Retrieve information from your mnemonic phrase.

5.  **-b / -balance (ADDRESS)**
	Check the balance of a specific wallet.
	

## Important Reminders and Security Practices

-   This tool is for research and security purposes *only*.
-   Never use this tool for illegal activities.
-   Secure your seed phrases.
-   Handle crypto with caution.
-   Keep the software updated.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code according to the terms of the license.