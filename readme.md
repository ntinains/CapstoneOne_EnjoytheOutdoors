# Capstone 2: Enjoy the Outdoors

Description: 

- HTML, CSS and JS project
- It involves finding national parks using dropdown selections
- There are three pages. A home page, national parks search page and a mountains information page 

## Pages 

### Home 
This is the landing page for our website and it includes navigation and highlights things people can to enjoy the great outdoors.

<p align="center" width="100%">
    <img width="70%" src="/Capstone Material/Screenshots/index.html"> 
</p>

### National Parks Search Page

<p align="center" width="100%">
    <img width="70%" src="/Capstone Material/Screenshots/National Parks page.PNG"> 
</p>

### Mountains Information Page


<p align="center" width="100%">
    <img width="70%" src="/Capstone Material/Screenshots/Mountainspage.PNG"> 
</p>

## Interesting Code Snipped 

What makes this code interesting is: 
- Easy to read.. Less Code
- Very efficient and very maintanable 
- It's also scalable

```
    const locations = [
        { name: "Rocky Mountain", type: "mountain", difficulty: "hard" },
        { name: "Yosemite", type: "park", size: "large" },
        { name: "Everest", type: "mountain", difficulty: "extreme" },
        { name: "Zion", type: "park", size: "medium" }
    ];

    const filteredMountains = filterLocations(locations, { type: "mountain" });
    console.log(filteredMountains);

    const difficultMountains = filterLocations(locations, { type: "mountain", difficulty: "hard" });
    console.log(difficultMountains);

-------------------------------------------------------------------------------------------------------------------
      let displayMountainInfo = () => {
    let selectedMountain = mountainSelectEl.value;
    descriptionEl.innerHTML = "";

    let mountainInfo = mountainsArray.find(
      (mountain) => mountain.name === selectedMountain
    );

    if (!mountainInfo) {
      descriptionEl.innerHTML = "No Mountain found";
    } else {
      let mountainHTML = `
        <p>Name: ${mountainInfo.name} </p>
        <p>Elevation: ${mountainInfo.elevation}</p>
        <p>Description: ${mountainInfo.desc}</p>
    `;

      descriptionEl.innerHTML += mountainHTML;
    }
  };

  mountainSelectEl.onchange = displayMountainInfo;
```




