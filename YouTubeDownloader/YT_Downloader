from pytube import YouTube

#Spør etter lenke fra bruker
path = input("Hvor vil du lagre filmen ? : ")
link = input("Link på video du vil laste ned:  ")
yt = YouTube(link)

#Detaljer om video som ønskes
print("Tittel ",yt.title)
print("Visninger på video ",yt.views)
print("Lengde på video",yt.length)
print("Vurderinger av videoen: ",yt.rating)
#Henter den høyeste oppløsningen av videoen
ys = yt.streams.get_highest_resolution()

#Startet downloading
print("Downloading...")
#Path til hvor den skal lagres
ys.download(path)
print("Download completed!!")