# slim Python base
FROM python:3.9-slim

WORKDIR /app

# आवश्यक फ़ाइलें कॉपी करें
COPY requirements.txt .

# dependencies इंस्टॉल करें
RUN pip install --no-cache-dir -r requirements.txt

# एप की सभी फाइलें कॉपी करें
COPY . .

# पोर्ट एक्सपोज़ करें
EXPOSE 5000

# कंटेनर के स्टार्टअप कमांड
CMD ["python", "app.py"]
