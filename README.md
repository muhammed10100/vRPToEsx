# vRPToEsx Lisans Haklarınca Bana Ayittir.
# MDT YAZILIM HİZMETLERİ.
# DİSCORD : discord.gg/TcrzQS7
# BENİM İZNİM OLMADAN BAŞKA BİR YERDE PAYLAŞILMASI YASAK.

--------------------------------------------------------------------------------------------------
Not bu kısmı  en üst kısmı full silin ve esx kısmını yapıştırın 
```lua
local Tunnel = module("vrp", "lib/Tunnel")
local Proxy = module("vrp", "lib/Proxy")

vRP = Proxy.getInterface("vRP")
vRPclient = Tunnel.getInterface("vRP","vrp_license")
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
ESX = nil

Citizen.CreateThread(function()
    while ESX == nil do
        TriggerEvent('esx:getSharedObject', function(obj) ESX = obj end)
        Citizen.Wait(0)
    end
end)
```

--------------------------------------------------------------------------------------------------

```lua
self:triggerEvent("ÖrenkCektirtme")
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
xPlayer.triggerEvent("ÖrenkCektirtme")
```

--------------------------------------------------------------------------------------------------
--Bildirim Kısmı --
```lua
vRPclient.notify(player,{"Örnek"})
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
TriggerEvent('Notification',"Örnek.")
```

--------------------------------------------------------------------------------------------------

```lua
vRP.getUserByRegistration()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
ESX.GetPlayerFromIdentifier()
```
--------------------------------------------------------------------------------------------------

Server dosya oyuncu çektirme.
```lua
vRP.getUserId()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
ESX.GetPlayerFromId()
```
--------------------------------------------------------------------------------------------------

```lua
vRP.getUserDataTable()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
ESX.GetPlayerData()
```
--------------------------------------------------------------------------------------------------

```lua
vRP.computeItemsWeight()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
xPlayer.setMaxWeight()
```
--------------------------------------------------------------------------------------------------

```lua
vRP.getItemWeight()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
xPlayer.getWeight()
```
--------------------------------------------------------------------------------------------------


```lua
vRP.hasPermission()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
xPlayer.getGroup()
```
--------------------------------------------------------------------------------------------------

```lua
vRP.tryFullPayment()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
-- test edilcek
xPlayer.getMoney()
```

--------------------------------------------------------------------------------------------------

```lua
vRP.setSData()
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
ESX.SetPlayerData()
```

--------------------------------------------------------------------------------------------------

```lua
vRP.kick(source, "Yazı <-> Text")
```
# ÜSTEKİ VRP

# ALTAKİ ESX
```lua
xPlayer.kick(source, "Yazı <-> Text")
```

--------------------------------------------------------------------------------------------------
ANİMASYON KSIMI SİZDE ÖRNEK VERDİM --- pek animasonlardan anlamam ama gerise bende :D.

```lua
vRP.playAnim(false,{{"mini@repair","fixing_a_player"}},true)
vRP.stopAnim(false)
```
# ÜSTEKİ VRP

# ALTAKİ ESX
https://docs.fivem.net/natives/?_0x9A2D0FB2E7852392
```lua
-- devamı gelcek
StopAnimTask(GetPlayerPed(-1), "mini@repair", "fixing_a_player", 1.0)
```
--------------------------------------------------------------------------------------------------




