# MoneyMaker 💸

Automate the creation of Tiktok locally, simply by providing a video topic to talk about.

# TODO

- [ ] Tiktok to douyin

## Installation 📥

`MoneyPrinter` requires Python 3.11 to run effectively.

After you finished installing Python, you can install `MoneyMaker` by following the steps below:

```bash
git clone https://github.com/kingbackyang/money_maker.git
cd MoneyPrinter

# Install requirements
pip install -r requirements.txt

# Copy .env.example and fill out values
cp .env.example .env

# Run the backend server
cd Backend
python main.py

# Run the frontend server
cd ../Frontend
python -m http.server 3000

# In mainland of China, need proxy. Pay attention to all the requests to/from sealand. You need to fill in the right proxy port. 
# e.g.
# openai.proxy = {
#    "http": "http://127.0.0.1:7890",
#    "https": "http://127.0.0.1:7890"}

# Moreover, to receive the response/get access to tiktok tts voice, you network proxy node address should be in America.
```

See [`.env.example`](.env.example) for the required environment variables.

If you need help, open [EnvironmentVariables.md](EnvironmentVariables.md) for more information.

## Usage 🛠️

1. Copy the `.env.example` file to `.env` and fill in the required values
1. Open `http://localhost:3000` in your browser
1. Enter a topic to talk about
1. Click on the "Generate" button
1. Wait for the video to be generated
1. The video's location is `MoneyMaker/output.mp4`

# Examples

-  https://www.tiktok.com/@offland123/video/7336180548424994081?is_from_webapp=1&sender_device=pc&web_id=7218823782936528427 (topic: how many mens have a guy they can call 3am?)
- https://www.tiktok.com/@offland123/video/7336184762119359776?is_from_webapp=1&sender_device=pc&web_id=7218823782936528427 (topic: Husband cheat on wife, and how to make them get back together)
- https://www.tiktok.com/@offland123/video/7336178720136383776?is_from_webapp=1&sender_device=pc&web_id=7218823782936528427 (topic: how to write a good CVPR paper)

