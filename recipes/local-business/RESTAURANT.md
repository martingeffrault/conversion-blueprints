# Restaurant & Food Service Recipe

> **Variant Focus**: Restaurants, cafes, bars, catering, food trucks
> **Examples**: McDonald's, Chipotle, local fine dining restaurants
> **Key Differentiator**: Menu-centric, location-focused, reservation/ordering integration
> **Revenue Model**: Dine-in, takeout, delivery, catering
> **Target**: Local customers, tourists, event planners

---

## How This Differs from Generic Local Business

| Aspect | Generic Local Business | Restaurant |
|--------|------------------------|------------|
| Hero CTA | "Contact Us" | "View Menu" or "Order Now" |
| Primary content | Services | Menu |
| Social proof | Reviews | Food photos + reviews |
| Conversion | Contact form | Reservations/online ordering |
| Location | Address + map | Address + map + hours + parking |
| Seasonality | Low | High (specials, seasonal menus) |

---

## Site Architecture

### Core Pages

```
/                       Homepage (ambiance, quick menu access)
├── /menu/              Full menu with categories
│   ├── /menu/lunch/    Daypart menus (optional)
│   ├── /menu/dinner/
│   └── /menu/drinks/
├── /reservations/      Booking page (OpenTable, Resy, direct)
├── /order/             Online ordering (if offered)
├── /about/             Story, chef, philosophy
├── /private-events/    Private dining, catering (if offered)
├── /gallery/           Food and ambiance photos
├── /contact/           Location, hours, parking
└── /gift-cards/        Gift card purchase (if offered)
```

### Optional Pages

```
├── /catering/          Catering services + menu
├── /blog/              Recipes, chef stories, events
├── /press/             Press mentions, awards
├── /careers/           Job openings
└── /locations/         Multi-location directory
```

---

## Homepage Structure

### Recommended Sections

```
1. Hero
   └── Ambiance image/video, tagline, primary CTA (Menu or Reserve)

2. Quick Actions (above fold on mobile)
   └── [View Menu]  [Make Reservation]  [Order Online]

3. About Teaser
   └── Brief story, philosophy, chef intro

4. Menu Preview
   └── Popular dishes or categories with photos

5. Location & Hours
   └── Map, address, hours, parking info

6. Social Proof
   └── Reviews, press mentions, awards

7. Instagram Feed (optional)
   └── Recent food photos

8. Newsletter/Offers (optional)
   └── Email signup for specials

9. Footer
   └── Contact, hours, social, legal
```

### Hero Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-screen ambiance image or video]                   │
│                                                                 │
│                                                                 │
│               Restaurant Name                                   │
│          "Tagline or cuisine type"                              │
│                                                                 │
│         [View Menu]     [Reserve a Table]                       │
│                                                                 │
│         Open Now · Closes 10 PM                                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Menu Page Patterns

### Menu Display Options

**Option 1: Category Cards**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Our Menu                                                       │
│                                                                 │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐               │
│  │ [Image]    │  │ [Image]    │  │ [Image]    │               │
│  │ Appetizers │  │ Mains      │  │ Desserts   │               │
│  └────────────┘  └────────────┘  └────────────┘               │
│                                                                 │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐               │
│  │ [Image]    │  │ [Image]    │  │ [Image]    │               │
│  │ Wine       │  │ Cocktails  │  │ Kids       │               │
│  └────────────┘  └────────────┘  └────────────┘               │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Option 2: Full Menu with Categories**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Appetizers] [Mains] [Desserts] [Drinks]  ← Sticky nav        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  APPETIZERS                                                     │
│  ───────────                                                    │
│                                                                 │
│  Bruschetta                                          $12       │
│  Tomatoes, basil, garlic, olive oil                            │
│  (V) (GF available)                                            │
│                                                                 │
│  Calamari Fritti                                     $16       │
│  Crispy fried calamari, marinara, lemon aioli                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Menu Item Information

| Element | Purpose |
|---------|---------|
| Name | Item identifier |
| Price | Clear pricing |
| Description | Ingredients, preparation |
| Dietary tags | (V) (VG) (GF) (DF) (N) |
| Photo (optional) | Visual appeal |
| Spice level | 🌶️ indicators |

### Dietary Legend

```
(V) Vegetarian    (VG) Vegan    (GF) Gluten-Free
(DF) Dairy-Free   (N) Contains Nuts
🌶️ Mildly spicy   🌶️🌶️ Medium   🌶️🌶️🌶️ Hot
```

---

## Reservation Integration

### Booking Options

| Platform | Best For | Integration |
|----------|----------|-------------|
| OpenTable | Fine dining, high volume | Widget embed |
| Resy | Trendy, urban restaurants | Widget embed |
| Yelp Reservations | SMB restaurants | Widget embed |
| Direct form | Full control | Custom form |
| Phone only | Traditional, high-touch | Phone number prominent |

### Reservation Page Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Reserve Your Table                                             │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  │        [OpenTable/Resy Widget Embed]                      │ │
│  │                                                           │ │
│  │   Party Size ▼    Date 📅    Time ▼                      │ │
│  │                                                           │ │
│  │             [Find a Table]                                │ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  Prefer to call? (555) 123-4567                                │
│                                                                 │
│  Private events? Contact our events team →                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Online Ordering Integration

### Ordering Platforms

| Platform | Type | Best For |
|----------|------|----------|
| Toast | POS + online | Full-service restaurants |
| Square Online | POS + online | Cafes, quick service |
| ChowNow | Commission-free | SMB restaurants |
| Direct integration | Custom | Large chains |
| Third-party links | Aggregators | DoorDash, UberEats links |

### Order Page Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Order Online                                                   │
│                                                                 │
│  [Pickup]  [Delivery]                                          │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  │  [Menu categories + items]                                │ │
│  │                                                           │ │
│  │  [Cart sidebar or bottom bar]                            │ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  Also available on:  [DoorDash]  [UberEats]  [Grubhub]        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Location & Hours

### Essential Information

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Visit Us                                                       │
│                                                                 │
│  ┌──────────────────────────────┐  123 Main Street             │
│  │                              │  City, State 12345           │
│  │      [Google Map]            │                              │
│  │                              │  ☎️ (555) 123-4567           │
│  │                              │                              │
│  └──────────────────────────────┘  [Get Directions]            │
│                                                                 │
│  HOURS                              PARKING                     │
│  ─────                              ───────                     │
│  Monday - Thursday: 5pm - 10pm      Street parking available   │
│  Friday - Saturday: 5pm - 11pm      Valet on weekends ($10)    │
│  Sunday: 4pm - 9pm                  Lot behind building        │
│                                                                 │
│  ⚠️ Reservations recommended for weekends                      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Multi-Location Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Our Locations                                                  │
│                                                                 │
│  [Search by city or ZIP]                                       │
│                                                                 │
│  ┌──────────────────┐  ┌──────────────────┐                   │
│  │ Downtown         │  │ Uptown           │                   │
│  │ 123 Main St      │  │ 456 Park Ave     │                   │
│  │ Open Now         │  │ Opens at 5pm     │                   │
│  │ [Details]        │  │ [Details]        │                   │
│  └──────────────────┘  └──────────────────┘                   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Social Proof for Restaurants

### Review Integration

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  What Guests Say                                                │
│                                                                 │
│  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐   │
│  │ [Google]       │  │ [Yelp]         │  │ [TripAdvisor]  │   │
│  │ ★★★★★ 4.7     │  │ ★★★★☆ 4.5     │  │ ★★★★★ 4.8     │   │
│  │ 500+ reviews   │  │ 300+ reviews   │  │ 200+ reviews   │   │
│  └────────────────┘  └────────────────┘  └────────────────┘   │
│                                                                 │
│  "Amazing food and atmosphere!" - John D. via Google           │
│  "Best Italian in the city" - Sarah M. via Yelp                │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Press & Awards

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Recognition                                                    │
│                                                                 │
│  🏆 Best New Restaurant 2024 - City Magazine                   │
│  ⭐ Michelin Bib Gourmand 2024                                 │
│  📰 "Must-Try" - Local Newspaper                               │
│                                                                 │
│  [Logo] [Logo] [Logo] [Logo]  ← Press logos                   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Local SEO for Restaurants

### Google Business Profile

Essential information:
- Accurate name, address, phone (NAP)
- Correct category (Restaurant, Cafe, etc.)
- Complete hours (including special hours)
- Menu link or menu items
- High-quality photos (food, interior, exterior)
- Regular posts (specials, events)
- Review responses

### Schema Markup

```json
{
  "@type": "Restaurant",
  "name": "Restaurant Name",
  "servesCuisine": "Italian",
  "priceRange": "$$",
  "address": {...},
  "telephone": "+1-555-123-4567",
  "openingHoursSpecification": [...],
  "menu": "https://restaurant.com/menu/",
  "acceptsReservations": "True"
}
```

### Local Keywords

| Type | Examples |
|------|----------|
| Cuisine + location | "Italian restaurant downtown" |
| Feature + location | "outdoor dining [city]" |
| Occasion + location | "date night restaurant [city]" |
| Near me | "restaurants near me" (GMB optimization) |

---

## Mobile Optimization

### Mobile Priorities

1. **Click-to-call** - Phone number tappable
2. **Click-to-directions** - Direct to maps app
3. **Menu accessible** - Easy to read on phone
4. **Sticky CTAs** - Reserve/Order always visible
5. **Fast loading** - Optimize images

### Mobile-First Navigation

```
┌────────────────────────────────────────┐
│  [Logo]                      [Menu ☰] │
├────────────────────────────────────────┤
│                                        │
│        [Page Content]                  │
│                                        │
├────────────────────────────────────────┤
│  [Menu]  [Reserve]  [Order]  [Call]   │ ← Sticky bottom bar
└────────────────────────────────────────┘
```

---

## Implementation Checklist

### Foundation
- [ ] Mobile-first responsive design
- [ ] Fast page speed (image optimization)
- [ ] SSL certificate
- [ ] Google Business Profile claimed

### Content
- [ ] Full menu with prices
- [ ] High-quality food photography
- [ ] About/story page
- [ ] Location with map and hours

### Functionality
- [ ] Reservation system integrated
- [ ] Online ordering (if applicable)
- [ ] Contact form
- [ ] Newsletter signup

### SEO
- [ ] Restaurant schema markup
- [ ] Local keywords optimized
- [ ] Google Business Profile optimized
- [ ] Reviews enabled and monitored

---

## Sources

- [Google - Local Business Guidelines](https://support.google.com/business)
- [OpenTable - Restaurant Marketing](https://restaurant.opentable.com/)
- [Toast - Restaurant Website Guide](https://pos.toasttab.com/)
- [National Restaurant Association](https://restaurant.org/)
