### @explicitHints 1
### @flyoutOnly true

# Espías

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
    cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireLegs(Legs.OverFourLegs), cyber.requireHoldingItem(HoldingItem.NoItem)))
    cyber.addDenyFirewallRule(cyber.requireEyewear(WearingEyeware.WearingEyeware))
})

```

## Espías @showdialog
Cuidado: se sabe que el reino rival intenta colar espías por nuestras puertas.   
![Espías](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_5.jpg)  


## ¡Espías!
Asegúrate de no dejar entrar a los espías: se disfrazan para que no los reconozcan.   
¿Cómo podríamos distinguirlos de los aldeanos normales?   


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireHat(WearingHat.NoHat), cyber.requireHoldingItem(HoldingItem.NoItem)))
})
```

### ~ tutorialhint
¿Qué llevan siempre los espías cuando quieren ocultar quiénes son?

```package
ciberseguridad-es=github:avilesalexmj-dev/minecraft-ciberseguridad-es
```
