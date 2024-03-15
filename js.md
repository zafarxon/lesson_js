```C
// 
for (let i = 0; i < assa.length; i = i + 1) {
  if (typeof assa[i] == "object") {
    for (let f = 0; f < assa[i].length; f = f + 1) {
      assa[i][f] = assa[i][f] * 2;
    }
  } else {
    assa[i] = assa[i] * 2;
  }
}

// 
function moreTwoTime(assa) {
  for (let i = 0; i < assa.length; i = i + 1) {
    if (typeof assa[i] == "object") {
      moreTwoTime(assa[i])
    } else {
      assa[i] = assa[i] * 2;
    }
  }

  return assa
}

// 
let assa = [2, 4,[2, 4, 3, 5, [2, 4, 3, 5, 6 ,3, 3,4,4,5,5] ,3, 3,4,4,5,5], 3, 5, 6 ,3, 3,4,4,5,5];
```

