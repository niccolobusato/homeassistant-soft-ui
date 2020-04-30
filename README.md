# homeassistant-soft-ui

requires card_mod to works

```css
style: |
  ha-card {
      background-color: var(--primary-background-color);
      border-radius: 15px;
      margin: 20px;
      box-shadow: 
           {% if is_state('sun.sun', 'above_horizon') %}
               -8px -8px 8px 0 rgba(255,255,255,.5),8px 8px 8px 0 rgba(0,0,0,.03);
           {% else %}
               -8px -8px 8px 0 rgba(50, 50, 50,.5),8px 8px 8px 0 rgba(0,0,0,.15);
           {% endif %}   
   }
```
