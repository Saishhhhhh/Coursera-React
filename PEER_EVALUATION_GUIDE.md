# Peer Evaluation Guide - Paradise Nursery Shopping Application

## Quick Testing Checklist for Peer Evaluators

### 🚀 **Getting Started**
1. **Clone/Download** the repository
2. **Install dependencies**: `npm install`
3. **Start the app**: `npm run dev`
4. **Open browser**: Navigate to `http://localhost:5173`

---

## 📋 **Systematic Testing Guide**

### **1. Landing Page Verification (5 points)**

#### ✅ **Background Image** (1 point)
- [ ] Beautiful greenhouse background image is visible
- [ ] Image covers the entire landing page
- [ ] Proper overlay and blur effects applied

#### ✅ **Company Information** (2 points)
- [ ] Company name "Paradise Nursery" is displayed
- [ ] Tagline "Where Green Meets Serenity" is visible
- [ ] AboutUs section contains company description
- [ ] Text is readable and properly styled

#### ✅ **Get Started Button** (2 points)
- [ ] Button is visible and clickable
- [ ] Clicking transitions to product listing page
- [ ] Smooth animation during transition

---

### **2. Product Listing Page Verification (9 points)**

#### ✅ **Plant Display** (2 points)
- [ ] At least 6 unique houseplants are displayed
- [ ] Each plant shows: thumbnail, name, description, price
- [ ] Images are high-quality and properly sized

#### ✅ **Categories** (1 point)
- [ ] Plants are organized into at least 3 categories
- [ ] Categories are clearly labeled
- [ ] 5 categories visible: Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, Low Maintenance

#### ✅ **Add to Cart Functionality** (6 points)
- [ ] Each plant has an "Add to Cart" button
- [ ] **Test**: Click "Add to Cart" on any plant
  - [ ] Shopping cart icon badge increases by 1
  - [ ] Button becomes disabled (shows "Added to Cart")
  - [ ] Plant appears in shopping cart
- [ ] **Test**: Try clicking the same button again
  - [ ] Button remains disabled
  - [ ] No duplicate items added

---

### **3. Header Navigation Verification (7 points)**

#### ✅ **Header Display** (2 points)
- [ ] Header appears on product listing page
- [ ] Header appears on shopping cart page
- [ ] Consistent styling across both pages

#### ✅ **Shopping Cart Icon** (3 points)
- [ ] Cart icon is visible in header
- [ ] **Test**: Add items to cart
  - [ ] Cart badge shows correct total number
  - [ ] Badge updates in real-time
- [ ] **Test**: Remove items from cart
  - [ ] Badge decreases accordingly
  - [ ] Badge disappears when cart is empty

#### ✅ **Navigation** (2 points)
- [ ] "Plants" link navigates to product page
- [ ] "Cart" link navigates to shopping cart page
- [ ] Company logo links back to landing page

---

### **4. Shopping Cart Page Verification (23 points)**

#### ✅ **Cart Summary** (4 points)
- [ ] Total number of plants displayed
- [ ] Total cost of all items displayed
- [ ] Both values update in real-time

#### ✅ **Cart Item Display** (6 points)
- [ ] Each plant type shows thumbnail image
- [ ] Each plant type shows name
- [ ] Each plant type shows unit price
- [ ] Layout is clean and organized

#### ✅ **Quantity Controls** (8 points)
- [ ] **Increase Button Test**:
  - [ ] Click "+" button on any item
  - [ ] Quantity increases by 1
  - [ ] Total cost updates
  - [ ] Cart badge updates
- [ ] **Decrease Button Test**:
  - [ ] Click "-" button on any item
  - [ ] Quantity decreases by 1
  - [ ] Item removes when quantity reaches 0
  - [ ] All totals update correctly

#### ✅ **Delete Functionality** (2 points)
- [ ] Each item has a "Delete" button
- [ ] **Test**: Click "Delete" on any item
  - [ ] Item completely removes from cart
  - [ ] Cart totals update
  - [ ] Cart badge updates

#### ✅ **Action Buttons** (3 points)
- [ ] **Continue Shopping Button**:
  - [ ] Button is visible
  - [ ] Clicking navigates back to product page
- [ ] **Checkout Button**:
  - [ ] Button is visible
  - [ ] Clicking shows "Coming Soon" alert

---

### **5. Redux Implementation Verification (4 points)**

#### ✅ **Redux Files** (4 points)
- [ ] `src/store.js` exists and properly configured
- [ ] `src/CartSlice.jsx` contains all required reducers
- [ ] `src/main.jsx` has Redux Provider setup
- [ ] Cart state persists across page navigation

---

## 🔧 **Technical Verification**

### **Redux State Management**
- [ ] Cart items are stored in Redux state
- [ ] Adding items updates Redux state
- [ ] Removing items updates Redux state
- [ ] Quantity changes update Redux state

### **Responsive Design**
- [ ] **Desktop**: All elements properly sized and positioned
- [ ] **Tablet**: Layout adapts to medium screens
- [ ] **Mobile**: Layout stacks properly on small screens
- [ ] **Touch-friendly**: Buttons are appropriately sized for touch

### **User Experience**
- [ ] Smooth animations and transitions
- [ ] Visual feedback on button interactions
- [ ] Proper loading states
- [ ] Accessibility features (focus states, contrast)

---

## 📊 **Scoring Guide**

### **Point Allocation**
- **GitHub Repository**: 6 points
- **Landing Page**: 5 points  
- **Product Listing Page**: 9 points
- **Header**: 7 points
- **Shopping Cart Page**: 23 points

### **Total**: 50 points

### **Grading Criteria**
- **Full Points**: Feature works exactly as specified
- **Partial Points**: Feature mostly works but has minor issues
- **No Points**: Feature missing or not functional

---

## 🐛 **Common Issues to Check**

1. **Cart State Persistence**: Ensure cart items remain when navigating between pages
2. **Button States**: Verify "Add to Cart" buttons become disabled after use
3. **Real-time Updates**: All totals should update immediately when cart changes
4. **Responsive Design**: Test on different screen sizes
5. **Navigation**: All links should work properly

---

## ✅ **Final Verification**

Before submitting your evaluation, ensure you have:
- [ ] Tested all 19 tasks
- [ ] Verified all 50 points
- [ ] Checked responsive design
- [ ] Tested all user interactions
- [ ] Verified Redux implementation

**The application should provide a smooth, professional shopping experience with all functionality working as specified in the requirements.** 