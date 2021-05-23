# vRPToEsx Lisans Haklarınca Bana Ayittir.
# BENİM İZNİM OLMADAN BAŞKA BİR YERDE PAYLAŞILMASI YASAK.

--------------------------------------------------------------------------------------------------
Not bu kısmı  en üst kısmı full silin ve esx kısmını yapıştırın 
```lua
MySQL = module("vrp_mysql", "MySQL")
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




