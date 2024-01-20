FROM python as pyth-image
WORKDIR /var/lib
COPY ./dummy.py .
RUN python dummy.py > log.txt
FROM ubuntu as main-cont
COPY --from=pyth-image /var/lib/log.txt /root
WORKDIR /root
CMD ["ls"]
