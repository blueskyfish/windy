
![Windy Layout](./logo-144.png)

# Windy Layout


## Global

| Name        | Value | Description     |
|-------------|-------|-----------------|
| font-family |       | The font family |
| font-size   |       |                 |
| gap         |       | The Gap         |
|             |       |                 |


## Button / Link

| Name          | Value | Description |
|---------------|-------|-------------|
| font-size     |       |             |
| padding x / y |       |             |
| border-radius |       |             |
| border        |       |             |
| background    |       |             |
| color         |       |             |
| hover         |       |             |
| focus         |       |             |
| active        |       |             |
| disabled      |       |             |

**Example**

```scss
.button, .btn {
  --wy-button-border-width: 1px;
  --wy-button-border-style: solid;
  --wy-button-border-color: var(--wy-grey-300);
  --wy-button-radius: var(--wy-gap-1);
  --wy-button-bg-color: var(--wy-grey-300);
  --wy-button-text-color: var(--wy-black);
  --wy-button-font-size: var(--wy-font-size);
  --wy-button-y-gap: var(--wy-gap-1);
  --wy-button-x-gap: var(--wy-gap-2);
  --wy-button-active-bg-color: var(--wy-grey-400);
  --wy-button-active-border-color: var(--wy-grey-400);
  --wy-button-active-text-color: var(--wy-black);
  --wy-button-focus-bg-color: var(--wy-grey-400);
  --wy-button-focus-border-color: var(--wy-grey-400);
  --wy-button-focus-text-color: var(--wy-black);
  --wy-button-disabled-bg-color: var(--wy-grey-50);
  --wy-button-disabled-border-color: var(--wy-grey-100);
  --wy-button-disabled-text-color: var(--wy-grey-300);
  
  border: var(--wy-button-border-width) var(--wy-button-border-style) var(--wy-button-border-color);
  border-radius: var(--wy-button-radius);
  background: var(--wy-button-bg-color);
  color: var(--wy-button-text-color);
  cursor: pointer;
  font-size: var(--wy-button-font-size);
  padding: var(--wy-button-y-gap) var(--wy-button-x-gap);
  
  &:active {
    background: var(--wy-button-active-bg-color);
    border-color: var(--wy-button-active-border-color);
    color: var(--wy-button-active-text-color);
  }
  
  &:focus {
    background: var(--wy-button-focus-bg-color);
    border-color: var(--wy-button-focus-border-color);
    color: var(--wy-button-focus-text-color);
  }
  
  &[disabled="true"] {
    background: var(--wy-button-disabled-bg-color);
    border-color: var(--wy-button-disabled-border-color);
    color: var(--wy-button-disabled-text-color);
    cursor: not-allowed;
  }
}

.button, .btn {
  &.blue {
    --wy-button-border-color: var(--wy-blue);
    --wy-button-bg-color: var(--wy-blue);
    --wy-button-text-color: var(--wy-white);
    --wy-button-active-bg-color: var(--wy-blue-600);
    --wy-button-active-border-color: var(--wy-blue-600);
    --wy-button-active-text-color: var(--wy-white);
    --wy-button-focus-bg-color: var(--wy-blue-700);
    --wy-button-focus-border-color: var(--wy-blue-700);
    --wy-button-focus-text-color: var(--wy-white);
    --wy-button-disabled-bg-color: var(--wy-blue-100);
    --wy-button-disabled-border-color: var(--wy-blue-100);
    --wy-button-disabled-text-color: var(--wy-grey-400);
    &.outline {
      --wy-button-bg-color: var(--wy-white);
      --wy-button-active-bg-color: var(--wy-blue-200);
      --wy-button-focus-bg-color: var(--wy-blue-200);
      --wy-button-disabled-bg-color: var(--wy-grey-100);
      --wy-button-disabled-text-color: var(--wy-grey-400);
    }
  }
  &.red {
    
  }
  &.green {
    
  }
}

```