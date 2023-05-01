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
