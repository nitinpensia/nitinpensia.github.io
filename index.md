---
layout: "default"
title: "🚀 kcm-kafka-connect-adls-sink - Easily Send Data to Azure"
description: "📝 Write Kafka records to Azure Data Lake Storage Gen2 using a Sink Connector with SAS authentication, supporting Avro and GZIP compression."
---
# 🚀 kcm-kafka-connect-adls-sink - Easily Send Data to Azure

## 🌐 Overview
The kcm-kafka-connect-adls-sink is a Kafka Connect Sink designed to help you easily send data from Kafka to Azure Data Lake Storage Gen2 (ADLS Gen2). It supports SAS authentication, handles Avro data formats, compresses data using GZIP, and organizes your data into partitions. This application simplifies data transfer and enhances your data storage solutions.

## 👨‍💻 Features
- **SAS Authentication**: Securely connect to ADLS Gen2 using SAS tokens.
- **Avro Support**: Store data in a compact and efficient Avro format.
- **GZIP Compression**: Reduce storage size with built-in GZIP compression.
- **Partition-Based File Batching**: Automatically group data into manageable files.

## 📦 System Requirements
To run the kcm-kafka-connect-adls-sink, ensure your system meets these requirements:
- **Java 8 or later**: This application runs on Java, so make sure you have a compatible version installed.
- **Kafka**: A running Kafka cluster is necessary for this application to send data.
- **Internet Connection**: You will need access to Azure services.

## 📥 Download & Install
To get started, visit the Releases page to download the application. 

[![Download kcm-kafka-connect-adls-sink](https://img.shields.io/badge/Download%20kcm--kafka--connect--adls--sink-blue.svg)](https://github.com/nitinpensia/kcm-kafka-connect-adls-sink/releases)

1. Click the button above or follow this link: [Download here](https://github.com/nitinpensia/kcm-kafka-connect-adls-sink/releases).
2. On the Releases page, find the latest version of the kcm-kafka-connect-adls-sink.
3. Select the appropriate file for your operating system.
4. Download the file to your computer.
5. Open the downloaded file to install or run the application. Follow any on-screen prompts.

## ⚙️ Configuration
After downloading, you need to configure the application to connect to your Kafka and Azure accounts.

1. **Create a Configuration File**: 
   You need a configuration file that specifies how the application connects to Kafka and ADLS Gen2. Create a text file named `kafka-connect-adls-sink.properties`.

2. **Add the Required Properties**: 
   In the configuration file, include the following properties:
   ```properties
   name=kcm-kafka-connect-adls-sink
   connector.class=com.nitinpensia.kafka.connect.adls.sink.AdlsSinkConnector
   tasks.max=1
   topics=your-kafka-topic
   adls.url=https://youraccount.dfs.core.windows.net/
   adls.sas.token=your-sas-token
   ```
   Replace `your-kafka-topic`, `youraccount`, and `your-sas-token` with your actual Kafka topic name, Azure Data Lake account, and SAS token.

3. **Run the Application**: 
   After setting up your configuration file, launch the kcm-kafka-connect-adls-sink application. It will start sending data from Kafka to ADLS Gen2 based on your configurations.

## 🔍 Troubleshooting
If you encounter issues, check the following:
- Ensure that your Java version is compatible.
- Validate the configuration file for errors.
- Confirm that your Kafka cluster is running and accessible.

Common errors may include authentication failures, network issues, or incorrect file paths.

## 📚 Support
For any support needs, feel free to raise issues on our [GitHub Issues page](https://github.com/nitinpensia/kcm-kafka-connect-adls-sink/issues). We aim to address queries promptly.

## 🛠️ Contributing
Contributions are welcome! If you have enhancements or bug fixes, please create a pull request or open an issue for discussion.

## ✉️ Feedback
Your feedback is valuable. Please share your thoughts or suggestions directly on the GitHub repository.

## 🌟 License
This project is licensed under the MIT License. You are free to use, modify, and distribute it in accordance with the license. 

Visit the Releases page to start utilizing the kcm-kafka-connect-adls-sink today!

[Download here](https://github.com/nitinpensia/kcm-kafka-connect-adls-sink/releases)