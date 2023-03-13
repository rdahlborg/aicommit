# AI Commit
Description
AI Commit is a command-line tool that automates the process of generating commit messages based on changes made to a Git repository using OpenAI's language models. It uses the Git diff command to get the changes, sends them to the OpenAI API, and receives a commit message suggestion in response. The script then amends the most recent Git commit with the generated commit message. This can save time and effort when committing changes to a Git repository, as it removes the need to manually write commit messages for each change.

### Commands

- `aicommit`: Show the commit message and exit.
- `aicommit commit`: Commit using an AI-generated commit message.

### Options

- `-h, --help`: Show this help message and exit.
- `--prefix`: Specify the type of commit (i.e. fix, feat, refactor, ticket number) to override the auto type. Default: auto.
- `--max_tokens`: Controls the maximum number of tokens to generate in the text completion task. Default: 100.
- `-d, --debug`: Debug.
- `--language`: Language for generated commit messages. Overrides the value of the system local `LANG` environment variable. Default: `<system local>`.

## Linux / MacOS Set-up

1. Clone the repository: `git clone https://github.com/username/aicommit.git`
2. Navigate to the directory: `cd aicommit`
3. Make the script executable: `chmod +x aicommit`
4. Add a PATH to your .bashrc or .bash_profile file: `echo "export PATH=\$PATH:$(pwd)" >> ~/.zshrc`
5. Run the following command in your terminal, replacing yourkey with your [API key](https://platform.openai.com/account/api-keys) `echo "export OPENAI_API_KEY='yourkey'" >> ~/.zshrc`
6. Refresh your shell environment: `source ~/.zshrc`
7. Run the script: `./aicommit --help`
 
Congratulations, you've successfully installed AI Commit! You can now run the aicommit command from anywhere in your terminal.
