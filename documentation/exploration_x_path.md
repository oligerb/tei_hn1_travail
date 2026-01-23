Sur cette page, vous trouvez quelques requêtes X path effectuées dans le logiciel BaseX.


Pour sortir les éléments de mes balises:

NATURE
<ul>
{
 for $nat in //seg[@ana='#NAT']/text()
  return <li>{data($nat)}</li>
}</ul>

AMOUR
<ul>
{
 for $amo in //seg[@ana='#AMO']/text()
  return <li>{data($amo)}</li>
}</ul>

DOULEUR
<ul>
{
 for $dol in //seg[@ana='#DOL']/text()
  return <li>{data($dol)}</li>
}</ul>


Pour sortir les thèmes utilisés:

for $theme in //interpGrp[@type="themes"]/interp let $id := concat("#", $theme/@xml:id) return <details> <summary>{string($theme)}</summary> <ul> { for $s in //seg[@ana = $id] return <li>{string($s)}</li> } </ul> </details>