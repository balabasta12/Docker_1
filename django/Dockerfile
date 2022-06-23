FROM python:3.8

WORKDIR /django

COPY . .

RUN pip install -r requirements.txt

ENV SECRET_KEY gk23k3fii#@@kjjfksdklfkdslfklkgrekopy''s\\fgddwer+rhgdfg\wer3i4558idrgwk
ENV DEBUG 1

RUN python manage.py migrate

#CMD ["gunicorn", "--bind", "0.0.0.0:8000", "stocks_products.wsgi"]
CMD ["python", "manage.py", "runserver","0.0.0.0:8000"]
