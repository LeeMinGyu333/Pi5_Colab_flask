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
wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-arm64.zip
unzip ngrok-stable-linux-arm64.zip
chmod +x ngrok
./ngrok version
/ngrok config add-aututoken^C
./ngrok authtoken 2yoIjXbMUtHCNk8MgxhKZMxODGd_7EiTpsT4Frm5CZVx47sit
./ngrok http 5000
