elb2s3failover.template
=============

Configures Route53 to provide failover beween an ELB and an S3 hosted static website.

Requirements
------------
You must have an existing S3 bucket configured as a Webhost, an existing Elastic Load Balancer, and an existing host zone in Route53.


Parameters
----------
#### elb2s3failover.template
<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>ELBDnsName</tt></td>
    <td>String</td>
    <td>Your ELB's DNS Name</td>
    <td><tt>none</tt></td>
  </tr>
  <tr>
    <td><tt>ELBHostedZoneID</tt></td>
    <td>String</td>
    <td>Your ELB's Hosted Zone ID</td>
    <td><tt>none</tt></td>
  </tr>
  <tr>
    <td><tt>HostedZoneName</tt></td>
    <td>String</td>
    <td>Your Hosted zone's name. Should end with a period after the TLD.</td>
    <td><tt>none</tt></td>
  </tr>
  <tr>
    <td><tt>DNSRecordName</tt></td>
    <td>String</td>
    <td>The name of the DNS record to do failover for. NOTE: Your S3 bucket name must match this. Should end with a period after the TLD.</td>
    <td><tt>none</tt></td>
  </tr>
  <tr>
    <td><tt>S3BucketRegion</tt></td>
    <td>String</td>
    <td>The S3 API region that your bucket lives in. US-Standard is us-east-1.</td>
    <td><tt>none</tt></td>
  </tr>
</table>
