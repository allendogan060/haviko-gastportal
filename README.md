# Haviko Gastportal

`gastportal.haviko.de` ist der persönliche Bereich für Restaurantgäste.

- Digitale Rechnungen werden über einen zufälligen QR-/Link-Token geladen.
- Die E-Mail-Anmeldung verwendet einen Supabase Magic Link.
- Angemeldete Gäste sehen nur Reservierungen und Besuche, deren bestätigte
  E-Mail-Adresse exakt zu ihrem Auth-Konto passt.
- Es gibt bewusst kein öffentliches Restaurant- oder Gästeverzeichnis.

## Veröffentlichung

1. Den Inhalt dieses Ordners als eigenes GitHub-Pages-Deployment veröffentlichen.
2. In GitHub Pages `gastportal.haviko.de` als Custom Domain eintragen und HTTPS aktivieren.
3. In IONOS einen CNAME `gastportal` auf `allendogan060.github.io` setzen.
4. Die SQL-Datei `Restaurant/supabase/guest_portal_migration.sql` in Supabase ausführen.
5. Unter Supabase Auth > URL Configuration `https://gastportal.haviko.de/` als Redirect URL ergänzen.
