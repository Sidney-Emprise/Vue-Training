
<template>
    <div>
        <ol>
        <li><slot name = "point"></slot>
          <ul>
            <li><slot name="details"></slot></li>
          </ul>
        </li>
        <li><strong>Analyze the user's problem and clarify it</strong></li>
          <ul>
            <li>Restate the problem to the user to ensure full understanding</li>
            <li>This eliminates assumptions and ensures clarity before proceeding with design</li>
          </ul>
      </ol>

      <i>
        <slot name="icon"></slot>
      </i>
      <div class="details">
        <h3>
          <slot name="heading"></slot>
        </h3>
        <slot></slot>
      </div>
    </div>
  </template>
  
  <style scoped>
  .item {
    margin-top: 2rem;
    display: flex;
    position: relative;
  }
  
  .details {
    flex: 1;
    margin-left: 1rem;
  }
