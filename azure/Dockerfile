
FROM gsusmita/my_app
WORKDIR /app
ARG SCRIPT_NAME
ENV SCRIPT=${SCRIPT_NAME}
RUN pip install dotenv
COPY helper.py /app 
COPY script_dir/${SCRIPT_NAME} /app
COPY env/config.env /app
CMD python ${SCRIPT} >> output.txt ; echo "Fetching Response"; python helper.py

