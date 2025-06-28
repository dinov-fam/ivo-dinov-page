# Ivo Dinov's Page

## Instructions: Separate Repositories

Each family member gets their own repository and full control over their subdomain.

### Step 1: Create New Repository for Ivo

1. Create new repository named `ivo-dinov-page`
2. Save the source HTML as `index.html` in this GitHub repository
3. Add a CNAME file containing: `ivo.dinov.org`

### Step 2: Enable GitHub Pages

1. Go to repository Settings \> Pages
2. Source: Deploy from a branch
3. Branch: main
4. Folder: / (root)
5. Custom domain `ivo.dinov.org`

### Step 3: DNS Configuration in GoDaddy

Add this CNAME record:
```
Type: CNAME
Name: ivo
Value: dinov-fam.github.io
TTL: 3600
```

The complete DNS setup will be:
```
Type: A, Name: @, Value: 185.199.108.153
Type: A, Name: @, Value: 185.199.109.153  
Type: A, Name: @, Value: 185.199.110.153
Type: A, Name: @, Value: 185.199.111.153
Type: CNAME, Name: www, Value: dinov-fam.github.io
Type: CNAME, Name: ivo, Value: dinov-fam.github.io
```

### Step 4: Repeat for Other Family Members

**For Darina:
- Repository: `darina-dinov-page`
- CNAME file: `darina.dinov.org`
- DNS: `Type: CNAME, Name: ina, Value: dinov-fam.github.io`

For Anna-Sophia:
- Repository: `anna-sophia-dinov-page`
- CNAME file: `anna-sophia.dinov.org`
- DNS: `Type: CNAME, Name: anna-sophia, Value: dinov-fam.github.io`

**For Kosta:**
- Repository: `kosta-dinov-page`
- CNAME file: `kosta.dinov.org`
- DNS: `Type: CNAME, Name: kosta, Value: dinov-fam.github.io`

## Recommended Setup Process

### Start with Ivo's Page:

1. Create repository: `ivo-dinov-page`
2. Add the HTML file I created above as `index.html`
3. Add CNAME file with content: `ivo.dinov.org`
4. Enable GitHub Pages with custom domain: `ivo.dinov.org`
5. Add DNS record in GoDaddy: `CNAME, ivo, [username].github.io`
6. Wait 15-30 minutes for propagation
7. Test: `https://ivo.dinov.org`

### Then Expand:
- Repeat the process for each family member
- Each gets their own repository and full control
- Easy to maintain and update individually

## Testing the Setup

### Expected Results:
- `dinov.org` → Main family page
- `ivo.dinov.org` → Ivo's personal page
- `darina.dinov.org` → Darina's personal page
- `anna-sophia.dinov.org` → Anna-Sophia's personal page
- `kosta.dinov.org` → Kosta's personal page

### Timeline:
- DNS propagation: 15 minutes - 2 hours
- HTTPS certificates: 1-24 hours
- Full functionality: Usually within 1-2 hours

## Updating Content:
- Each family member can update their own repository
- Changes reflect automatically on their subdomain
- No need to coordinate with others

### Adding New Family Members:
1. Create new repository: `[name]-dinov-page`
2. Add CNAME file with `[name].dinov.org`
3. Add DNS record in GoDaddy
4. Enable GitHub Pages

This approach gives you maximum flexibility and makes it easy for each family member to maintain their own professional presence while being part of the family website network!

