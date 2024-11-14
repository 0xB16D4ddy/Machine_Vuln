# Use the Metasploitable2 image from Docker Hub as the base image
FROM tleemcjr/metasploitable2:latest

# # Create a log file and set permissions
# RUN mkdir -p /var/log && touch /var/log/metasploitable.log && \
#     chmod 666 /var/log/metasploitable.log

# Run the Metasploitable services and keep the container running
CMD ["/bin/bash", "-c", "/bin/services.sh && tail -f /dev/null"]
