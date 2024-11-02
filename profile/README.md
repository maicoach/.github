# Maicoach project

This is the root of the MIACOACH project. The intention is to build the next generation of AI powerd sports coaching. 

The project consists of a Expo React native mobile app that runs on both Android and iOS. The backend is hosted on Google Cloud platform, with all infrastructure declared using terraform in the maicoach-gcp project. 
The remaining repositories are all Google Cloudrun Functions the together make up the API backend. 

The infrastructure is currently very simple, with DNS pointing to an API gateway where the SSL certificate is terminated and connections are routed to the functions. 
Data is stored as json documents in firebase, with workouts stored in cloud storage buckets. 
