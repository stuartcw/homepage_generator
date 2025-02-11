# Homepage Generator

A tool to generate a static HTML locally that your browser opens as its default page.

README for Static Dashboard Generator

## Overview

Static Dashboard Generator is a Python-based tool for generating a local static HTML file that acts as your browser’s default homepage. Designed as a personalized work dashboard, it aggregates useful information from various sources, including:

* Files you recently worked on.
* Current projects derived from a .doing.md file in your work folders.
* RSS feed headlines and other data sources.
* A plugin system for user-specific extensions.

The tool empowers users to stay organized by presenting a snapshot of their work, ongoing tasks, and useful links on a single, visually appealing dashboard.

### Features
1. Dynamic Content Aggregation
	* Tracks and displays recently accessed files.
	* Parses .doing.md files in designated folders to identify active projects.
2. RSS Feed Integration
	* Fetches and displays the latest headlines from RSS feeds.
3. Customizable Plugin System
	* Extend the dashboard’s functionality by creating custom plugins to integrate new data sources.
4. Simple HTML Output
	* Generates a static HTML file that is visually appealing and compatible with modern browsers.
	* Automatically sets the file as the browser’s default homepage for immediate accessibility.
5. Local Operation
	* Runs entirely on your machine; no internet connection is required for core functionalities.

## Requirements
* Python 3.7 or higher
* An installed browser for viewing the generated dashboard
* Required Python packages (install via pip):
* feedparser (for RSS integration)
* jinja2 (for templating the HTML output)
* watchdog (optional, for monitoring file changes)

# Installation
* lone the repository:
 
```bash
git clone https://github.com/yourusername/static-dashboard-generator.git
cd static-dashboard-generator
```

2.	Install dependencies:
 
```bash
pip install -r requirements.txt
```

3.	Run the tool to generate your dashboard:

```bash
python generate_dashboard.py
```

4.	Set the output HTML file (e.g., dashboard.html) as your browser’s default homepage.

## Usage

### Configuration
	
1.	Tracking .doing.md Files
Specify the directories to monitor in the config.json file. The tool will parse .doing.md files in these directories for project information.
2.	RSS Feeds
Add the URLs of your favorite RSS feeds to the config.json file to include their headlines on the dashboard.
3.	Custom Plugins
Place your custom plugins in the plugins/ directory. Plugins must follow the template provided in the documentation.

### Running the Tool
* To generate the dashboard:

```bash
python generate_dashboard.py
```

* To monitor file changes and auto-update the dashboard (optional):

```
python monitor.py
```

## Ideas for Future Development

1. Interactive Features
	* Support for updating .doing.md entries directly from the dashboard.
	* Add task-tracking functionality with checkboxes and progress bars.
2. Theme Customization
	* Allow users to select or create their own dashboard themes (e.g., dark mode).
3. Enhanced File Tracking
	* Display frequently accessed files and their edit history.
	* Add search functionality for files and projects.
4. Improved Plugin System
	* Add a web-based interface to enable or configure plugins.
	* Offer a plugin marketplace for sharing user-created plugins.
5. Additional Data Sources
	* Integrate with popular APIs (e.g., Google Calendar, GitHub, Jira).
	* Allow importing data from CSV or JSON files.
6. Widgets and Modules
	* Add weather, stock prices, or news modules.
	* Include productivity timers or focus widgets.
7. Mobile Compatibility
	* Generate responsive designs for viewing on mobile devices.
8. Notifications and Alerts
	* Notify users about upcoming deadlines, meetings, or task updates.
	* Integrate desktop notifications for urgent RSS headlines.
9. Version Control Support
	* Display Git commit history or repository activity for tracked projects.
10. Performance Optimizations
	* Minimize HTML size for faster loading times.
	* Cache RSS feed results to reduce network overhead.

## Contributing

Contributions are welcome! Please follow these steps:
1.	Fork the repository and create a new branch for your feature or bug fix.
2.	Submit a pull request with a detailed description of the changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to suggest new features or report bugs by opening an issue on the GitHub repository.
