FROM amazon/aws-lambda-provided:al2

WORKDIR /var/runtime/
COPY bootstrap bootstrap
RUN chmod 755 bootstrap

WORKDIR /var/task/
COPY function.sh function.sh
RUN chmod 755 function.sh

CMD [ "function.sh.handler" ]
