# Impostor: Track Leaks, Find Culprits

Impostor is a powerful CLI based file-sharing and tracking tool designed to help you find the source of leaks in your documents. Built using Go, it offers seamless integration with SMTP servers for automatic file sharing and tracking. With Impostor, you can protect your sensitive documents and quickly identify the responsible person in case of a data breach.

## Features

- **File Sharing**: Easily share files with multiple recipients securely.
- **Signature Generation**: Generates unique signatures for each recipient and embeds them into the shared file secretly.
- **SMTP Integration**: Automate file sharing by integrating with SMTP servers for email delivery.
- **Cross-Platform Compatibility**: Works with every file type and provides additional features for common file types such as PDF, DOCX, MOV, etc.
- **Leak Tracking**: Quickly identify the source of a document leak by comparing signatures stored in the database.

## Getting Started

### Prerequisites

- Go installed on your system.

### Installation

1. Clone the Impostor repository to your local machine:

   ```bash
   git clone https://github.com/your-username/impostor.git
   ```

2. Navigate to the project directory:

   ```bash
   cd impostor
   ```

3. Build the Impostor binary:

   ```bash
   go build
   ```

### Usage

1. Share a File:
   
   To share a file, run the Impostor binary with the path to the file and a list of recipients:

   ```bash
    go run main.go -n <name-of-project> -f <path-to-file> -t targets.txt 
   ```

2. Track a Leak:

   To track a leak and find the responsible person, provide the leaked file to Impostor:

   ```bash
    go run main.go -n <name-of-project> -f <path-to-file> -validate
   ```
