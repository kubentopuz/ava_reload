import requests
import threading
import time
def process_data(telegram_id):
    headers = {
        'Accept': 'application/json, text/plain, */*',
        'Accept-Encoding': 'gzip, deflate, br, zstd',
        'Accept-Language': 'en-US,en;q=0.9',
        'Content-Length': '46',
        'Content-Type': 'application/json',
        'Referer': 'https://bot.ethernity.game/',
        'sec-ch-ua': '"Chromium";v="124", "Microsoft Edge";v="124", "Not-A.Brand";v="99", "Microsoft Edge WebView2";v="124"',
        'sec-ch-ua-mobile': '?0',
        'sec-ch-ua-platform': '"Windows"',
        'Sec-Fetch-Dest': 'empty',
        'Sec-Fetch-Mode': 'cors',
        'Sec-Fetch-Site': 'same-origin',
        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36',
    }

    json_data = {
        'additionalTime': 3600,
        'telegramId': auth,
    }

    response = requests.post('https://bot.ethernity.game/api/add-mining-time', headers=headers, json=json_data)
    print(response.text)

with open('dataava.txt', 'r') as file:
            for line in file:
                telegram_id = line.strip().split('|')
                threading.Thread(target=process_data, args=(telegram_id)).start()
            time.sleep(5)
