# LWC/LWR Quick Reference Cheat Sheet

## NPM Commands

### Development
```bash
npm install                  # Install all dependencies
npm run dev                  # Start development server (http://localhost:3000)
npm run build               # Build for production
npm start                   # Start production server
```

### Maintenance
```bash
npm outdated                # Check for outdated packages
npm update                  # Update packages
npm audit                   # Check for vulnerabilities
npm audit fix               # Fix vulnerabilities automatically
npm cache clean --force     # Clear npm cache
```

## Testing Checklist

### Before Commit
- [ ] `npm run build` succeeds
- [ ] No console errors in browser
- [ ] Components render correctly
- [ ] Events work as expected
- [ ] Responsive design works
- [ ] Code is formatted

### Before Deploy
- [ ] Build succeeds
- [ ] Test in production mode locally
- [ ] Check all routes work
- [ ] Verify no hardcoded localhost URLs
- [ ] Update README if needed

## Useful Links

- LWC Documentation: https://lwc.dev/
- LWR Documentation: https://developer.salesforce.com/docs/platform/lwr/overview
- GitHub Pages Docs: https://docs.github.com/en/pages
- LWC Recipes: https://github.com/trailheadapps/lwc-recipes
- LWC Playground: https://developer.salesforce.com/docs/platform/lwc/guide/playground.html

## Quick Tips

1. **Component names must be kebab-case** in HTML: `<my-component>`
2. **Property names must be camelCase** in JS: `myProperty`
3. **HTML attributes must be kebab-case**: `parent-data={value}`
4. **Always use `key` in loops** for performance
5. **Events bubble by default** unless you call `stopPropagation()`
6. **Data binding is one-way** from parent to child
7. **Use CustomEvent** for child-to-parent communication
8. **@track is for objects/arrays**, primitive values are automatically reactive
9. **Component HTML must have single root** in template
10. **Cannot access DOM directly** except via `this.template.querySelector()`
