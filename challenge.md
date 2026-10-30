# Challenge: Environment Audit and Ping Block

## Job 1
Commands: printenv | grep PATH ; printenv | grep LANG ; printenv | grep PWD
PATH = /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/home/saraajmal30
LANG = en_US.UTF-8
PWD = /home/saraajmal30

## Job 2
Commands: export STUDENT_NAME="Sara" ; export STUDENT_ROLL_NUMBER="..." ; export STUDENT_SEMESTER="5" ; printenv | grep '^STUDENT_'
Logout/login ke baad grep khali aaya, kyunke export temporary hai.

## Job 3
Commands: teen export lines ~/.bashrc mein add ki ; source ~/.bashrc ; printenv | grep '^STUDENT_'
Naye login ke baad values maujood thin.

## Job 4
Commands: sudo cp /etc/ufw/before.rules ~/before.rules.backup ;
sudo sed -i (echo-request line par ACCEPT ko DROP) ; sudo ufw reload
Ping (PC se): Request timed out.
Undo: sed se DROP ko ACCEPT ; sudo ufw reload ; ping dobara chala.
