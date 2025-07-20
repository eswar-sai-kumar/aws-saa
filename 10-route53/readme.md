# Route53

- Route53 → Hosted zones → eswarsaikumar.site

<img width="1402" height="726" alt="image" src="https://github.com/user-attachments/assets/a6c57835-004a-4e47-8232-12cb886788b0" />

- Create record

<img width="1552" height="702" alt="image" src="https://github.com/user-attachments/assets/87664c9c-9c48-47a4-9c8a-5c14941fa16a" />

- Enter record name, record type, value (EC2 IP), TTL(60sec, not 300)    →   Create records 

<img width="1867" height="637" alt="image" src="https://github.com/user-attachments/assets/d16165a0-4699-4fa9-9234-5d4d175b27e4" />

- Open example.eswarsaikumar.site in browser

<img width="578" height="235" alt="image" src="https://github.com/user-attachments/assets/ea2734c0-310b-4e06-b402-f0123f303ecb" />

## Route 53 - TTL

Create another EC2 instance, update "example.eswarsaikumar.site" record value as new IP, check example.eswarsaikumar.site in browser

- Before 60 sec (TTL)

<img width="617" height="235" alt="image" src="https://github.com/user-attachments/assets/d81f5a01-f74d-4cca-9f43-b0ffe451b7a3" />

- After 60 sec

<img width="592" height="206" alt="image" src="https://github.com/user-attachments/assets/2d22f686-2be9-4f9a-aa9a-77ff40ad9369" />

## Route53 - ALB

- Create Load balancer after creating target group

- Create record → alias (Alias to Application and classical Load Balancer)  → Create Record




