# Secure Communication

This project implements a secure communication system using encryption, decryption, and digital signatures to ensure the confidentiality and integrity of messages. It uses CryptoJS for cryptographic operations and JSEncrypt for handling digital signatures.

## Features

- **Encryption and Decryption**: Utilizes AES encryption to securely transmit messages.
- **Digital Signatures**: Ensures the authenticity and integrity of messages using RSA digital signatures.
- **User Interface**: Simple and intuitive UI for sending and receiving encrypted messages.

## Getting Started

### Prerequisites

- A modern web browser that supports JavaScript.
- Internet connection to load external CryptoJS and JSEncrypt libraries.

### Installation

Clone the repository to your local machine:

```sh
git clone https://github.com/rae3skhan/Digital-Signature.git

```


Navigate to the project directory:

```sh
cd Digital-Signature
```

### Usage

Open the `index.html` file in your web browser to start the application. Enter your message, select a recipient, and click "Send Encrypted Message" to see the encryption and digital signature process in action.


## Key Management

Adding Public and Private Keys
To integrate your public and private keys into the system:

Generate your keys following the provided instructions.
Insert your public key and private key into the designated sections of the code, replacing the placeholders.
Generating Keys

Private Key

Generate a private key using OpenSSL:
```bash
openssl genpkey -algorithm RSA -out private_key.pem -pkeyopt rsa_keygen_bits:2048
```

Public Key

Extract the public key from the private key:

```bash
openssl rsa -pubout -in private_key.pem -out public_key.pem
```

## Built With

- [CryptoJS](https://cryptojs.gitbook.io/docs/) - Used for encryption and decryption.
- [JSEncrypt](https://github.com/travist/jsencrypt) - Used for creating and verifying digital signatures.

## Contributing

Please read [CONTRIBUTING.md](https://github.com/rae3skhan/Digital-Signature/blob/main/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors

- **Raees Khan** - *Initial work* - [Raees Khan](https://github.com/rae3skhan)

See also the list of [contributors](https://github.com/rae3skhan/Digital-Signature/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.


This README provides a basic overview of the project, including how to get started, the technologies used, and how to contribute. Adjustments can be made based on the project's evolution and specific requirements.