# Temple Gold

A wedding invitation website for a South Indian temple wedding: light the lamp,
the temple bell rings, the doors open, and the invitation unfolds.

**Demo (Ananya & Karthik):** https://choprakhushee.github.io/Temple-Gold/invites/ananya-weds-karthik/

Status: the entry (lamp, bell and temple doors) is finished. The invitation
sections are being built next. A full, plain-language guide comes with them.

## How it's organised

```
templates/temple-gold/        the design, shared by every couple who picks it
  assets/elements/            drop Canva elements here (see the README inside)
  sample-wedding.json         sample details for a new couple
templates/shared/             the foundation shared by all templates
invites/<couple>/             one folder per couple: index.html + wedding.json
tools/new-invite.py           creates a couple's folder
```

## Adding a new couple

```
python3 tools/new-invite.py aisha-weds-rahul
```

Edit `invites/aisha-weds-rahul/wedding.json`, run the command again (it
refreshes the WhatsApp preview), then commit and push.
