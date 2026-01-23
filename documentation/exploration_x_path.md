Sur cette page, vous trouvez quelques requêtes X path effectuées dans le logiciel BaseX.


Pour sortir les éléments de mes balises:

<ul>
{
 for $nat in //seg[@ana='#NAT']/text()
  return <li><a href="premierdoc.xml#{data($nat)}">{data($nat)}</a></li>
}</ul>