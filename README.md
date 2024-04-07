
# Shell Script Project: GitHub Repository Access Information

In this project, I have developed a shell script to retrieve information about users who have read access to a specific repository on GitHub.

## Implementation Instructions:
1. Clone this repository to your local machine using the following command in your terminal:
git clone <link_of_this_repository>
2. Set up your GitHub username and personal access token:
- Export your GitHub username to a shell variable named `username`:
  ```
  export username="your_username"
  ```
- Generate a personal access token in your GitHub account:
  - Navigate to GitHub > Settings > Developer settings > Personal access tokens > Generate new token.
  - Select the appropriate scopes for your token (e.g., `repo` for accessing repositories).
  - Copy the generated token.

3. Export your GitHub personal access token to a shell variable named `token`:

  export token="your_personal_access_token"

4. Give execute permission to the shell script:
  chmod +x list-users.sh (chmod 777 list-users.sh)

5. Run the shell script with the organization name and repository name as arguments:
  ./list-users.sh organization_name repository_name

Replace `organization_name` and `repository_name` with the respective values for the GitHub organization and repository you want to retrieve information for.

## Output:

The script will list the users with read access to the specified repository.

## Script Explanation:

- `list-users.sh`: The shell script file containing the code to retrieve repository access information.
- `API_URL`: The URL for GitHub API.
- `USERNAME`: Variable to store your GitHub username.
- `TOKEN`: Variable to store your GitHub personal access token.
- `REPO_OWNER` and `REPO_NAME`: Variables to store the organization name and repository name respectively.
- `github_api_get`: Function to make a GET request to the GitHub API.
- `list_users_with_read_access`: Function to list users with read access to the repository. (  if we removw jq in the function then output will be given in json format)
- Main script execution to display the output.

  
