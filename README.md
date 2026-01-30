# Automated Rain Alert using OpenWeatherMap & Twilio API

1. Create account on [openweathermap.org](https://openweathermap.org/)
2. Sign Up on [twilio.com](https://www.twilio.com/en-us) and get a free trial number

you can send message to any verified number in your twilio account

---

## Running on local machine

### Set Environment variables
Create .env file and add these environment variables

    OWM_API_KEY=your_openweathermap_api_key_here

    TWILIO_ACCOUNT_SID=your_twilio_account_sid_here
    TWILIO_AUTH_TOKEN=your_twilio_auth_token_here

    TWILIO_PHONE_NUMBER=your_twilio_phone_number_here
    RECIPIENT_PHONE_NUMBER=recipient_phone_number_here

**Create Python virtual environment**

    python3 -m venv .venv

**Activate enironment**

    source .venv/bin/activate

**Intall required package**

    pip install -r ./requirements.txt

**Run python main file**

    python3 main.py

---

## Running on pythonanywhere server

1. Create account on [pythonanywhere.com](https://www.pythonanywhere.com/)

2. copy paste pythonanywhere.py to a main file of a project on pythonanywhere site 

3. Copy paste your account_sid from and to numbers

4. export env variables

    Task -> Schedule task -> Command 

        export OWM_API_KEY="VALUE"; export AUTH_TOKEN="VALUE"; python3 main.py

5. Schedule Time to run python script

    Task -> Schedule task -> Set Time (UTC)