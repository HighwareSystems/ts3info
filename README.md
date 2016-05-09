# ts3info
Sencillo script que usa JQUERY principalmente para ver información sobre el estado de un servidor de Teamspeak 3.
El estado del servidor se comprueba a través de la API de <a href="https://www.planetteamspeak.com/">PlanetTeamspeak.com</a>, que interactúa directamente con la lista pública de servidores de Teamspeak.

GET https://api.planetteamspeak.com/serverstatus/IP:PUERTO/

Con este script podrás ver los siguientes atributos del servidor:
<ul>
  <li><strong>Estado </strong><i>(json.status)</i><strong>.</strong></li>
  <li><strong>Nombre del servidor </strong><i>(json.result.name)</i><strong>.</strong></li>
  <li><strong>Dirección IP </strong><i>(json.result.address)</i><strong>.</strong></li>
  <li><strong>Usuarios:</strong> UsuariosActuales / UsuariosTotales <i>(json.result.users / json.result.slots)</i></li>
  <li><strong>Contraseña </strong><i>(json.result.password)</i><strong>:</strong> comprueba si el servidor de ts3 está protegido por contraseña.</li>
  <li><strong>Localización del servidor</strong><i> (json.result.country)</i><strong>:</strong> filtro por país.</li>
  <li><strong>Licencia </strong><i>(json.result.premium)</i><strong>:</strong> valores 'si' o 'no'.</li>
</ul>
