# Maccabee

Static HTML, CSS, and JavaScript site. Files live at the repository root. There is no build step.

This site was never on a public domain. It has no custom domain. Do not add one, turn on Netlify DNS, or change any nameservers. It lives only at https://maccabee.netlify.app.

## GitHub

- Repository: `ecotto7/maccabee` (public, under the `ecotto7` account, not BIG-IC).
- Branch: `main`.
- Deploys happen only by pushing to `main`.

## Netlify

- Team: Gonzo Systems. Team slug: `ecotto7`. Do not create the site on any other Netlify account.
- Site name: `maccabee`.
- Connected repository: `ecotto7/maccabee`.
- Build command: empty. Publish directory: `.`
- `netlify.toml` stays at the repo root with `publish = "."`.
- Do not run `netlify deploy`, `netlify deploy --prod`, or a deploy through the Netlify tools unless the owner explicitly asks. Each production deploy costs 15 credits from a shared 300-per-month pool. If that pool runs out, every site on the team pauses. The GitHub import is the production deploy.

## Pages

- Home, Maccabee, The Colony, The Comb, Honey, and The Swarm.
- Folder URLs: `/the-colony/` is `the-colony/index.html`. Do not rename or move a page without a 301 in `netlify.toml`.
- Keep the designed wording, including the existing typos.
- The footer line is `© Adults Who Make Bad Decisions`. Do not add a year.
- Keep mailto links as mailto links.

## Forms

The contact form on The Swarm stays on its existing provider. It is the Elementor form already on the site (`form_id` `461f1c8`, `post_id` `235`), and it posts to `https://btuxlscv.elementor.cloud/wp-admin/admin-ajax.php`.

Do not use Netlify Forms. Do not add `data-netlify`, a form-name field, or a honeypot. The hidden `form_fields[field_website]` input is already part of that Elementor form. Leave it in place.
