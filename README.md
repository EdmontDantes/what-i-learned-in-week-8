# what-i-learned-in-week-8

## How to use functions with DOM Javascript

We learned how to use function in a separate backend and frontent separate javascript files in order to make a functionality of a website with various outputs.

We achieve this with creating handler function that loop through the elements and create element and then add .addEventListener on various inputs of mouse or anything else like 'click'.

example of handler function from "How We Roll Assignment" :

```
const d6ClickHandlerFunc = function() {
  let random6numOutput = getRandomNumber(6);
  sixes.push(random6numOutput);
  idRollQueryForImgD6.src = `./images/d6/${random6numOutput}.png`;
  const sixesMean = mean(sixes);
  const sixesMedian = median(sixes);
  d6QueryForMean.innerText = sixesMean;
  d6QueryForMediam.innerText = sixesMedian;

}
```

example of .addEventListener :

``` button query   

const idRollQueryForImgD6 = document.querySelector('#d6-roll')


idRollQueryForImgD6.addEventListener('click', d6ClickHandlerFunc);

```

## Flex CSS

Flex CSS become flex CSS when you add to selector ```display: flex``` property. It works on two axis one is ```justify-content: row``` --- x axis and another ```justify-content: column```     