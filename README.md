#  Vehicle Scraper

A Python web scraper designed to extract vehicle listings data from a popular vehicle marketplace in Sri Lanka.

## 📋 Features

- Extracts detailed vehicle information from multiple pages of listings
- Captures comprehensive data including:
  - Vehicle make, model, and year
  - Price and location
  - Contact information
  - Technical specifications (engine size, mileage, fuel type)
  - Additional options and details
- Handles pagination to scrape multiple pages
- Implements appropriate request delays to respect the website's servers
- Exports data to CSV for easy analysis

## 🛠️ Requirements

- Python 3.6+
- Required packages:
  - requests
  - beautifulsoup4
  - pandas

## ⚙️ Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/dilanka-heshan/Vehicle-Scraper.git
   cd vehicle_scraper
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use: venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage

1. Run the main script:
   ```bash
   python vehicle_scraper.py
   ```

2. The script will:
   - Scrape the specified number of pages (configurable in the script)
   - Extract detailed information from each vehicle listing
   - Save the data to a CSV file (`vehicle_data.csv`)

3. Configure scraping parameters by editing the script:
   - Change `max_pages` to scrape more or fewer pages
   - Adjust the time delays between requests if needed

## 📊 Sample Output

The script generates a CSV file with columns including:

- Title
- Price
- Location
- Ad Date
- Contact
- Make
- Model
- YOM (Year of Manufacture)
- Mileage (km)
- Gear (Transmission)
- Fuel Type
- Engine (cc)
- Options
- Details
- Link

## ⚠️ Disclaimer

This scraper is for educational purposes only.  Consider the following ethical guidelines:

- Implement reasonable delays between requests
- Do not overload their servers with excessive requests
- Only scrape publicly available information
- Do not use the data for commercial purposes without permission

## 📜 License

[MIT License](LICENSE)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
