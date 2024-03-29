# Lab 10: Blockchain

## Run hash_value.py twice and compare results
```
$ cd ~/iot/lesson10
```
![image](https://user-images.githubusercontent.com/94701716/235464105-33b59a34-9dae-4ca5-accf-0accefa37ce6.png)

```
$ cat hash_value.py
```
![image](https://user-images.githubusercontent.com/94701716/235464359-b5d62a7e-fa5a-4499-92f3-95cae79581d4.png)

```
$ py hash_value.py
```
![image](https://user-images.githubusercontent.com/94701716/235464576-d583f88e-db8f-446a-acf1-268a9320887b.png)

```
$ py hash_value.py
```
![image](https://user-images.githubusercontent.com/94701716/235465027-cd7d41dd-009f-462b-9535-74c897462148.png)

## Run snakecoin.py
```
$ cat snakecoin.py
```
![image](https://user-images.githubusercontent.com/94701716/235466928-f55a6489-0a40-4579-833c-0f104aee6963.png)

```
$ py snakecoin.py
```
![image](https://user-images.githubusercontent.com/94701716/235467246-788fde9b-3184-46e2-bcec-48d558813035.png)
![image](https://user-images.githubusercontent.com/94701716/235467331-32d86e5c-5842-43c8-943a-d04e7a2d643c.png)

## Run snakecoin-server-full-code.py on Terminal 1 and mine a new block on Terminal 2
```
$ py snakecoin-server-full-code.py
```
![image](https://user-images.githubusercontent.com/94701716/235470375-30d60bf7-fdb5-4394-8e8e-bd46163be529.png)

```
$ curl "localhost:5000/txion" \
     -H "Content-Type: application/json" \
     -d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'
$ curl localhost:5000/mine
```
![image](https://user-images.githubusercontent.com/94701716/235471095-1cdbdc02-614c-41b0-af06-b2e74d8ec6e4.png)
![image](https://user-images.githubusercontent.com/94701716/235471312-ecf4cee5-b384-4388-b4b5-0f8eee177033.png)

## Clone Python blockchain app and uncomment the last line of node_server.py
```
$ git clone https://github.com/satwikkansal/python_blockchain_app.git
```
![image](https://user-images.githubusercontent.com/94701716/235475065-7cb96d53-b4d4-441a-a804-0d7fed4c2fcb.png)

```
$ cd ~/python_blockchain_app
```
![image](https://user-images.githubusercontent.com/94701716/235475389-8796cb20-95cb-48b3-af92-bc303c5f7c42.png)

```
$ nano node_server.py
```
![image](https://user-images.githubusercontent.com/94701716/235475848-24841a5f-c4c4-42dc-8bea-fc0cf38820b3.png)
![image](https://user-images.githubusercontent.com/94701716/235475712-4023ebc7-bf68-4fc1-9af9-7bd7aa4bf93e.png)

## Run node_server.py on Terminal 1 and run_app.py on Terminal 2
```
$ py node_server.py
```
![image](https://user-images.githubusercontent.com/94701716/235476544-44449e55-71c1-434c-9620-6d0143d10bca.png)

```
$ vncserver
$ cd ~/python_blockchain_app
$ python3 run_app.py
```
![image](https://user-images.githubusercontent.com/94701716/235478797-f03e2b08-6bf5-4e8e-8b88-31ccea4b26c0.png)
![image](https://user-images.githubusercontent.com/94701716/235478853-dd2c09a1-eac5-45ad-8e54-5f63cddc30a2.png)
