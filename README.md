# kube.ipspeed.telefraf

echo "# kube.ipspeed.telefraf" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:thlasta/kube.ipspeed.telefraf.git
git push -u origin main

Repo clonen
git clone git@github.com:thlasta/kube.ipspeed.telefraf.git

# Repo auschecken/holen
git pull git@github.com:thlasta/kube.ipspeed.telefraf.git

# Bei Änderungen:
git commit -m "Änderungsbeschreibung"
git push --all

# Namespace "octoprint" anlegen
kubectl create namespace monitoring

# Jump one folder up, and apply to the whole folder:
kubectl apply -f ips.telegraf/