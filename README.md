# 1) Scraper for SRMAcademia ( [Academia](https://academia.srmist.edu.in/#) )

# Overview
 
This project is a web scraper built using Playwright and BeautifulSoup to automate the process of logging into the SRMIST portal, scraping the academic timetable data, academic calendar data and extracting relevant information such as subjects, slots, room numbers and other calendar data.


# Tech Stack
- **Python**
- **Playwright** : For browser automation
- **BeautifulSoup** : For parsing HTML and scraping data


# Installation

## 1. Clone the repository
```bash
git clone https://github.com/meyyappan055/AcademiaScraper.git
```

## 2. Install dependencies

```bash
pip install -r requirements.txt
```

## 3. Create a `.env` file

Create a `.env` file in the root directory and add your SRMIST login credentials:

```env
USERNAME= your_srmist_username
PASSWORD= your_srmist_password
```

## 4. Install Playwright Browsers

Playwright requires you to install browser binaries. Run the following command to install the necessary browsers:

```bash
python -m playwright install
```

## 5. Setup Cookies

On the first run, the script will log in to SRMIST and save the session cookies in `session_cookies.json`.  
This allows you to skip login in future runs.

## Usage

### 1. Running the test_login.py

```bash
cd app
python test_login.py
```


### 2. Running the Unified Timetable Scraper

Scrape the Unified Time Table for Batch 1 and Batch 2 :

```bash
cd unified_timetable_scraper
python test_unified_timetable.py
```

### 3. Running the User Timetable Scraper

This will return course title , slot and room number.

To scrape the timetable data, run the following:

```bash
cd user_timetable_scraper
python test_timetable_scraper.py
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

