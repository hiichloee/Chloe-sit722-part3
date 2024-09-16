
FROM python:3.9-slim

WORKDIR /app

COPY requirements.txt /app/

RUN pip install --no-cache-dir -r requirements.txt

COPY . /app

EXPOSE 8000

ENV DATABASE_URL=postgresql://hiichloee:6zNXaWkwpu0VLbK7P5mCRPIkVJcq43dY@dpg-crjt8rd2ng1s73fkfdcg-a.singapore-postgres.render.com/chloe_sit722_55is

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]

