FROM python:3.11 as builder

#TODO add build steps
# ----------------------
WORKDIR /html
COPY . .

FROM httpd:alpine
# COPY docs/_build/html/ /usr/local/apache2/htdocs/
# COPY --from=builder /usr/local/lib/python3.8/site-packages/ /usr/local/apache2/htdocs/
COPY --from=builder /html/ /usr/local/apache2/htdocs/