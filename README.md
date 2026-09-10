# Hive report — sign-in page

The sign-in page for the BLE link report. It holds nothing secret: the Supabase
anon key here is designed to be public and opens nothing on its own, because the
report requires a signed-in user's session.

Everything else — the report itself, the data, the gateway firmware — lives
elsewhere. This repo exists only because Supabase serves HTML as `text/plain`,
so the page that starts the sign-in needs a host that serves real HTML.

Generated from `supabase/functions/ble-report/login.html` in the (private)
gateway repo by `tools/deploy_report.sh login`. Edit it there, not here.
