Maak een OU aan in AD Users & Computers in de Root van de AD

Zorg nu dat  je het departement IT toevoegt, maar gebruik daarbij PATH om dit in de OU Sint-Niklaas te zetten

New-ADOrganizationalUnit -Name Sint-Niklaas
New-ADGroup -Name IT -path "ou=Sint-Niklaas, dc=mediatech, dc=LAN"
Add-ADGroupMember -Identity IT -Members BLC
