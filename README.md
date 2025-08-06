# SMS-Translation

SMS-Translation is a program that allows user to automatically translate their messages based on phone numbers. It translates the message according to which region the phone number belongs to using Amazon Translation. As a result, it outputs a txt file where translated versions of message and phone numbers are matched. This program is useful especially for companies or organizations that want to reach people from different countries using SMS.

## Features
- Users can choose a .txt file to determine phone numbers. Also, a default phone number list is provided. Suggestion for users is to determine their own list. 
- While entering messages, program checks character count and does not allow a message with more than 210 characters since SMS has a limit of 160 characters. After translating the message, program warns users if translated versions are longer than 160 characters. It provides some options to user convert message to camelCase, ignoring and adding to output as it is, or entering a new message.
- Users should determine input message's language for translation to be better.
- While writing their messages, users can change font size based on preferences.
- They can copy the message with one click.
- After writing their messages, they can translate this automatically for each phone number efficiently and output these translations to an output file in a directory where they choose.
- Also, users can change theme between light mode and dark mode. 

##### IT DOES NOT SEND SMSs FOR NOW.

## How to run program using an IDE:
Users shold have their own API keys for Amazon translation. 
-  Users should create their own Amazon API keys
-  Then:
-  "set AMAZON_API_KEY=your_api_key_here" and "set AMAZON_API_SECRET=your_api_secret_here" for Windows Command Prompt
-  "export AMAZON_API_KEY=your_api_key_here" and "export AMAZON_API_SECRET=your_api_secret_here" for macOS/Linux (bash or zsh)

Now, users can execute program with usage of dependencies

## How to run program directly:
- Users can directly execute "translate-app.jar" file if Java 21+ is downloaded on their systems. 
- If not, they need to download and execute.

## How is program designed:
This program is designed with Java. GUI of this program is designed with Java Swing library. This program also uses many libraries that you can find in dependencies section.

## Creators:
Talha Safa Küçük

## Dependencies:
            <groupId>software.amazon.awssdk</groupId>
            <artifactId>translate</artifactId>
            <version>2.20.100</version>

            <groupId>software.amazon.awssdk</groupId>
            <artifactId>auth</artifactId>
            <version>2.20.100</version>

            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-simple</artifactId>
            <version>2.0.9</version>

            <groupId>com.googlecode.libphonenumber</groupId>
            <artifactId>libphonenumber</artifactId>
            <version>8.13.14</version>
        
            <groupId>com.ibm.icu</groupId>
            <artifactId>icu4j</artifactId>
            <version>73.2</version>

            <groupId>com.formdev</groupId>
            <artifactId>flatlaf</artifactId>
            <version>3.4</version>
