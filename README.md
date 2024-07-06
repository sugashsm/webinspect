**WebInspect**
WebInspect is a browser forensics tool designed to extract and analyze browser data. It supports Firefox and Chrome and offers features to list browser profiles, view browsing history, downloads, and export data to CSV files.

Features
List browser profiles
View browsing history with filters
View downloaded files with filters
Export browser data to CSV files
Requirements
Python 3.x
Required Python libraries (see requirements.txt)
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/webinspect.git
cd webinspect
Install the required Python libraries:

bash
Copy code
pip install -r requirements.txt
Usage
To use WebInspect, run the script with the desired subcommand and options.

List Browser Profiles
bash
Copy code
python webinspect.py profiles
View Browsing History
bash
Copy code
python webinspect.py history --profile [PROFILE_ID] [--filter FILTER]
View Downloads
bash
Copy code
python webinspect.py downloads --profile [PROFILE_ID] [--filter FILTER]
Export Data
bash
Copy code
python webinspect.py export --profile [PROFILE_ID] --to [DESTINATION_PATH]
Command-Line Arguments
-v, --version: Show the current version of WebInspect
profiles: List browsers profiles
--id [ID]: Select profile by ID
history: View browsing history
--profile [ID]: Select profile by ID
--filter [FILTER]: Add filter to history output
--export [FILE]: Export output to CSV file
downloads: View downloaded files
--profile [ID]: Select profile by ID
--filter [FILTER]: Add filter to downloads output
export: Export profile data
--profile [ID]: Select profile by ID
--to [PATH]: Destination path for exported profile
Example
List all browser profiles:

bash
Copy code
python webinspect.py profiles
View browsing history for profile 1:

bash
Copy code
python webinspect.py history --profile 1
Export data for profile 1 to the "exports" directory:

bash
Copy code
python webinspect.py export --profile 1 --to ./exports
License
This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to customize this README as per your specific needs or additional details about the project. ​
