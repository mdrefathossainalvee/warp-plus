```markdown
# WARP-PLUS-CLOUDFLARE

## Overview

This script allows you to obtain unlimited WARP+ referral data from Cloudflare's WARP VPN service. It automates the process of sending requests to the WARP+ API using random client IDs and handles responses to add data to your WARP+ account.

## Features

- Generates random client IDs and tokens.
- Sends requests to Cloudflare's WARP+ API.
- Handles successful and unsuccessful responses.
- Configurable request intervals.
- Saves referral data to a file.

## Requirements

- Python 3.x
- `httpx` library (automatically installed if not found)
- `poetry` (if `httpx` needs to be installed)

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/WARP-PLUS-CLOUDFLARE.git
   cd WARP-PLUS-CLOUDFLARE
   ```

2. **Install dependencies:**
   ```sh
   pip install httpx
   ```

3. **Run the script:**
   ```sh
   python script.py
   ```

## Usage

1. **Start the Script:**
   - Run the script and choose option `1` to start.
   - If the referrer (user ID) is not set, you will be prompted to enter it.

2. **Set Minimum Request Interval:**
   - Choose option `2` to set the minimum interval between requests (in seconds).

3. **Set Maximum Request Interval:**
   - Choose option `3` to set the maximum interval between requests (in seconds).

4. **Set Referrer (User ID):**
   - Choose option `4` to set or change the referrer (user ID).

5. **Display Referral Data:**
   - Choose option `5` to display the referral data stored in the script.

6. **Exit the Script:**
   - Choose option `6` to exit the script.

## Script Details

The script consists of several functions and components:

- **Random String Generators:**
  - `genString(length)`: Generates a random alphanumeric string of the specified length.
  - `digitString(length)`: Generates a random numeric string of the specified length.

- **API Request:**
  - Sends a POST request to Cloudflare's WARP+ API with generated client IDs and tokens.
  - Handles responses and updates referral data.

- **Main Menu:**
  - Provides options to start the script, set intervals, set the referrer, display data, and exit.

- **Stop Function:**
  - Checks for user input to stop the script.

## Example Output

When running the script, you will see various outputs indicating the status of requests, such as:

```
[+] Sending request...
[-] WORK ON ID: your-referrer-id
[:)] Request completed successfully.
[:)] X GB has been successfully added to your account.
[#] Total: X Good Y Bad
[*] After Z seconds, a new request will be sent.
```

## Author

Made with ♡ by Mayday.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

This README file provides a comprehensive overview of your project, including installation instructions, usage details, and a description of the script's functionality. Adjust the text and sections as needed to fit your specific project and preferences.
