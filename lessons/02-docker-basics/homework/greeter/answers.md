docker build -t greeter:v1
docker run -d --name greeter -p 9000:8000 greeter:v1
greeting='shalom'
shalom Rivka
Docker שומר כל שורה ב-Dockerfile כשכבה ב-cache. כשמשהו משתנה, השורות שלפני השורה שהשתנתה נלקחות מה-cache, ואילו השורה שהשתנתה וכל השורות שאחריה רצות מחדש.