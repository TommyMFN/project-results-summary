# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

## Colors

### Primary

- Light red: hsl(0, 100%, 67%)
- Orangey yellow: hsl(39, 100%, 56%)
- Green teal: hsl(166, 100%, 37%)
- Cobalt blue: hsl(234, 85%, 45%)

## Gradients

- Light slate blue (background): hsl(252, 100%, 67%)
- Light royal blue (background): hsl(241, 81%, 54%)

- Violet blue (circle): hsla(256, 72%, 46%, 1)
- Persian blue (circle): hsla(241, 72%, 46%, 0)



### Neutral

- White: hsl(0, 0%, 100%)
- Pale blue: hsl(221, 100%, 96%)
- Light lavender: hsl(241, 100%, 89%)
- Dark gray blue: hsl(224, 30%, 27%)

### Notes

Use transparency to get the colour variations necessary to match the design. Hint: look into using `hsla()`.

## Typography

### Body Copy

- Font size (paragraphs): 18px

### Font

- Family: [Hanken Grotesk](https://fonts.google.com/specimen/Hanken+Grotesk)
- Weights: 500, 700, 800


Archive Code Media:

.parent-con {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  height: 100vh;
  border: 6.25rem;
  border-radius: 100%;

  .results-con {
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    justify-content: space-between;

    border-radius: 10px;
    height: 250px;
    width: 150px;
    margin: 10px;
    margin-right: 0px;
    padding: 25px;
    background-image: linear-gradient(
      to bottom,
      $gradient-light-state-blue-bg,
      $gradient-light-royal-blue-bg
    );

    h3 {
      color: $neutral-pale-blue;
    }

    .score-circle {
      h1 {
        font-size: 3.125rem;
        color: white;
      }

      display: flex;
      flex-direction: column;
      justify-content: center;
      align-self: center;
      font-size: 10px;
      border-radius: 50%;
      padding: 10px;
      text-align: center;
      width: 100px;
      height: 100px;
      font-family: "Hanken Grotesk", sans-serif;
      color: $neutral-pale-blue;
      background-image: linear-gradient(
        to bottom,
        $gradient-light-state-blue-bg,
        $gradient-light-royal-blue-bg
      );
    }

    h2 {
      margin: 10px;
      font-size: 20px;
      color: white;
    }

    p {
      color: $neutral-pale-blue;
      font-size: 0.625rem;
      font-weight: 500;
    }
  }

  .summary-con {
    display: flex;
    flex-direction: column;
    box-shadow: 0px 4px 1px rgba(0, 0, 0, 0.084);
    border-bottom-right-radius: 10px;
    background-color: rgb(255, 255, 255);
    .grid-container {
      display: grid;
      gap: 10px;
      padding: 10px;
      column-gap: 30px;

      .summary-header {
        color: $neutral-dark-gray-blue;
        font-weight: 700;
      }
      .highlight {
        color: $neutral-light-lavender;
        font-weight: bold;
      }

      .item1 {
        display: flex;
        align-items: center;
        grid-column-start: 1;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        color: $primary-light-red;
        font-weight: bold;
      }

      .item2 {
        display: flex;
        align-items: center;
        grid-column-start: 3;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        font-weight: bold;
        color: $neutral-dark-gray-blue;
      }

      .item3 {
        display: flex;
        align-items: center;
        grid-column-start: 1;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        color: $primary-orangey-yellow;
        font-weight: bold;
      }

      .item4 {
        display: flex;
        align-items: center;
        grid-column-start: 3;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        font-weight: bold;
        color: $neutral-dark-gray-blue;
      }

      .item5 {
        display: flex;
        align-items: center;
        grid-column-start: 1;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        color: $primary-green-teal;
        font-weight: bold;
      }

      .item6 {
        display: flex;
        align-items: center;
        grid-column-start: 3;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        font-weight: bold;
        color: $neutral-dark-gray-blue;
      }
      .item7 {
        display: flex;
        align-items: center;
        grid-column-start: 1;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        color: $primary-cobalt-blue;
        font-weight: bold;
      }
      .item8 {
        display: flex;
        align-items: center;
        grid-column-start: 3;
        grid-column-end: 3;
        padding: 10px;
        gap: 10px;
        font-weight: bold;
        color: $neutral-dark-gray-blue;
      }
    }

    .summary-footer {
      display: flex;
      justify-content: center;
      padding: 3px;
      margin: 10px;
      border-style: dotted;
      border-color: black;

      .summary-button {
        background-color: $neutral-dark-gray-blue;
        padding: 12px 24px;
        border: none;
        border-radius: 100px;
        width: 200px;
        color: white;
        font-weight: 700;
      }
    }
  }
}

