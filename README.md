#Install the Worker:

helm install prod-bowchat-worker ./prod-bowchat-worker -n prod-bowchat


#Upgrade:

helm upgrade prod-bowchat-worker ./prod-bowchat-worker -n prod-bowchat


#Scale workers:

helm upgrade prod-bowchat-worker ./prod-bowchat-worker \
  --set replicaCount=3 \
  -n prod-bowchat
