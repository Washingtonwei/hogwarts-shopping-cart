<template>
  <div class="shopping-cart">
    <h1>Harry's Shopping Cart</h1>
    <div class="cart-container">
      <div class="cart-list">
        <div class="cart-list-item">
          <img
            src="@/assets/img/DragonLiver.png"
            alt="Dragon Liver"
            class="product-image"
          />
          <div class="item-details-with-actions">
            <div class="item-details">
              <h2>Dragon Liver</h2>
              <p class="price">$1500</p>
              <p class="in-stock-status">
                <i class="fa-solid fa-check"></i> In stock
              </p>
            </div>
            <div class="item-actions">
              <div class="quantity-selector">
                <button class="quantity-change-button">−</button>
                <input
                  type="text"
                  class="quantity-input"
                  value="3"
                  aria-label="quantity"
                />
                <button class="quantity-change-button">+</button>
              </div>
              <button class="remove-item">✕</button>
            </div>
          </div>
        </div>
        <div class="cart-list-item">
          <img
            src="@/assets/img/GoldenSnitch.png"
            alt="Golden Snitch"
            class="product-image"
          />
          <div class="item-details-with-actions">
            <div class="item-details">
              <h2>Golden Snitch</h2>
              <p class="price">$600</p>
              <p class="in-stock-status">
                <i class="fa-solid fa-check"></i> In stock
              </p>
            </div>
            <div class="item-actions">
              <div class="quantity-selector">
                <button class="quantity-change-button">−</button>
                <input
                  type="text"
                  class="quantity-input"
                  value="2"
                  aria-label="quantity"
                />
                <button class="quantity-change-button">+</button>
              </div>
              <button class="remove-item">✕</button>
            </div>
          </div>
        </div>
        <div class="cart-list-item">
          <img
            src="@/assets/img/UnicornTailHair.png"
            alt="Unicorn Tail Hair"
            class="product-image"
          />
          <div class="item-details-with-actions">
            <div class="item-details">
              <h2>Unicorn Tail Hair</h2>
              <p class="price">$1200</p>
              <p class="on-backorder-status">
                <i class="fa-solid fa-hourglass-half"></i> On backorder
              </p>
            </div>
            <div class="item-actions">
              <div class="quantity-selector">
                <button class="quantity-change-button">−</button>
                <input
                  type="text"
                  class="quantity-input"
                  value="1"
                  aria-label="quantity"
                />
                <button class="quantity-change-button">+</button>
              </div>
              <button class="remove-item">✕</button>
            </div>
          </div>
        </div>
        <div class="cart-list-item">
          <img src="@/assets/img/Wand.jpg" alt="Wand" class="product-image" />
          <div class="item-details-with-actions">
            <div class="item-details">
              <h2>Wand</h2>
              <p class="price">$2000</p>
              <p class="in-stock-status">
                <i class="fa-solid fa-check"></i> In stock
              </p>
            </div>
            <div class="item-actions">
              <div class="quantity-selector">
                <button class="quantity-change-button">−</button>
                <input
                  type="text"
                  class="quantity-input"
                  value="1"
                  aria-label="quantity"
                />
                <button class="quantity-change-button">+</button>
              </div>
              <button class="remove-item">✕</button>
            </div>
          </div>
        </div>
        <div class="cart-list-item">
          <img
            src="@/assets/img/Nimbus2000.jpg"
            alt="Nimbus 2000"
            class="product-image"
          />
          <div class="item-details-with-actions">
            <div class="item-details">
              <h2>Nimbus 2000</h2>
              <p class="price">$5000</p>
              <p class="in-stock-status">
                <i class="fa-solid fa-check"></i> In stock
              </p>
            </div>
            <div class="item-actions">
              <div class="quantity-selector">
                <button class="quantity-change-button">−</button>
                <input
                  type="text"
                  class="quantity-input"
                  value="1"
                  aria-label="quantity"
                />
                <button class="quantity-change-button">+</button>
              </div>
              <button class="remove-item">✕</button>
            </div>
          </div>
        </div>
      </div>
      <div class="order-summary">
        <h2>Order summary</h2>
        <button class="toggle-details-button">Hide Details</button>
        <div class="">
          <div class="summary-item">
            <span>Subtotal</span>
            <span>$13900</span>
          </div>
          <div class="summary-item">
            <span>Shipping estimate</span>
            <span>$100</span>
          </div>
          <div class="summary-item">
            <span>Tax estimate</span>
            <span>$1112</span>
          </div>
        </div>
        <div class="summary-total">
          <strong>Order total</strong>
          <strong>$15112</strong>
        </div>
        <button class="checkout-button">Checkout</button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
/* Styles for the shopping cart */
.shopping-cart {
  font-family: 'Arial', sans-serif;
  background-color: #f8f8f8;
  margin: 0;
  padding: 0;
}

/* Styles for the cart title */
h1 {
  padding: 20px;
  max-width: 1200px;
  margin: auto;
}

/* Styles for the cart list and order summary */
.cart-container {
  display: flex;
  align-items: flex-start;
  max-width: 1200px;
  margin: auto;
}

.cart-list {
  flex-grow: 2;
  margin-right: 20px;
}

.order-summary {
  flex-basis: 300px;
  background-color: #f9fafb;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

/* Styles for the cart list item */
.cart-list-item {
  display: flex;
  align-items: center;
  background-color: #fff;
  margin-bottom: 10px;
  border-radius: 8px;
  padding: 10px;
}

.product-image {
  width: 100px;
  margin-right: 10px;
}

.item-details-with-actions {
  display: flex;
  flex-grow: 1;
  margin-left: 10px;
}

.item-details {
  flex-grow: 1;
}

.item-actions {
  display: flex;
  align-items: center;
}

.price {
  font-size: 0.9em;
  color: #666;
}

.in-stock-status {
  font-size: 0.9em;
  color: green;
}

.on-backorder-status {
  font-size: 0.9em;
  color: red;
}

.quantity-selector {
  display: flex;
  border: 1px solid #c1c1c1;
  border-radius: 8px;
  overflow: hidden;
  /* Ensures the children do not break the rounded corners */
}

.quantity-change-button {
  background-color: #ffffff;
  border: none;
  padding: 10px 12px;
  cursor: pointer;
  font-size: 1rem;
  transition: all 0.2s;
}

.quantity-input {
  border: none;
  text-align: center;
  width: 40px;
  padding: 10px;
  font-size: 1rem;
  transition: all 0.2s;
}

.quantity-input:focus {
  outline: none;
}

.remove-item {
  background: none;
  border: none;
  border-radius: 50%;
  cursor: pointer;
  font-size: 1.2em;
  margin-left: 20px;
}

.quantity-change-button:hover,
.quantity-change-button:focus,
.quantity-input:focus,
.remove-item:hover,
.remove-item:focus {
  background-color: #f2f2f2;
}

/* Styles for the order summary */
.toggle-details-button {
  background-color: #f1f1f1;
  color: #333;
  padding: 10px 15px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  margin-bottom: 10px;
}

.hide-order-details {
  display: none;
  /* Hide details by default */
}

.summary-item {
  display: flex;
  justify-content: space-between;
  padding: 10px 0;
}

.summary-total {
  display: flex;
  justify-content: space-between;
  font-weight: bold;
  padding: 10px 0;
  border-top: 1px solid #e2e2e2;
  margin-top: 10px;
}

.checkout-button {
  background-color: #4f46e5;
  color: #fff;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  width: 100%;
  cursor: pointer;
  margin-top: 10px;
  transition: all 0.2s;
  /* smooth transition in and out */
}

.checkout-button:hover {
  background-color: #4138d9;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}
</style>