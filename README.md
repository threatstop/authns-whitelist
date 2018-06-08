# authns-whitelist

This repo takes the TLD zone files and does a count of instances of specific authoritative nameservers used by domain. The concept is that if a nameserver provides authoritative resolution for 1M domains, great care should be taken before using that in RPZ (or using it's underlying IP address in RPZ or firewalls).  There are limitations to this approach and it is currently in experimental form.

Eventually these files will be updated on a daily basis, but for now, it is still a project in testing.

There are two files, one that has a unique count of nameservers in reverse order, and one that does the same thing for IP addresses for those underlying nameservers. There may be overlap (the same NS hostname could share IP addresses with multiple NS hostnames, for instance).

Questions should go to John Bambenek, VP of Security Research and Intelligence at ThreatSTOP (jbambenek /at\ threatstop \dot/ com).
