# Pi5_Colab_flask
# Ubuntu libraries
pip install flask
sudo apt update
sudo apt install python3-opencv
sudo apt install python3-gpiozero

#colab
!pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
!git clone https://github.com/ultralytics/yolov5
%cd yolov5
!pip install -r requirements.txt
pip install deep_sort_realtime
pip install opencv-python
pip install requests


#ngrok setting
cd ~
curl -s https://ngrok-agent.s3.amazonaws.com/ngrok.asc | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null && \
  echo "deb https://ngrok-agent.s3.amazonaws.com buster main" | sudo tee /etc/apt/sources.list.d/ngrok.list && \
  sudo apt update && sudo apt install ngrok
ngrok config add-authtoken 2yoIjXbMUtHCNk8MgxhKZMxODGd_7EiTpsT4Frm5CZVx47sit
ngrok http 5000

# u can see forwarding :" https:~~-free.app", copy https~app and paste to colab code
VIDEO_URL = "https~~free.app/video_feed"
