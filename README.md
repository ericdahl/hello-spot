# hello-spot

experiments with AWS Spot instances

## Notes

### 2023-10-29 selection

- requirements
    - accelerator max = 0
    - vcpu max = 4
    - memory_ max = 16 GB
    - memory_gb_per_cpu = 4

| Instance Type  | Description | vCPUs | Memory (GB) |
|----------------|-------------|-------|-------------|
| a1.large        |             | 2     | 4           |
| a1.medium       |             | 1     | 2           |
| a1.xlarge       |             | 4     | 8           |
| c1.medium       |             | 2     | 2           |
| c3.large        |             | 2     | 4           |
| c3.xlarge       |             | 4     | 8           |
| c4.large        |             | 2     | 4           |
| c4.xlarge       |             | 4     | 8           |
| c5.large        |             | 2     | 4           |
| c5.xlarge       |             | 4     | 8           |
| c5a.large       |             | 2     | 4           |
| c5a.xlarge      |             | 4     | 8           |
| c5ad.large      |             | 2     | 4           |
| c5ad.xlarge     |             | 4     | 8           |
| c5d.large       |             | 2     | 4           |
| c5d.xlarge      |             | 4     | 8           |
| c5n.large       |             | 2     | 5           |
| c5n.xlarge      |             | 4     | 11          |
| c6a.large       |             | 2     | 4           |
| c6a.xlarge      |             | 4     | 8           |
| c6g.large       |             | 2     | 4           |
| c6g.medium      |             | 1     | 2           |
| c6g.xlarge      |             | 4     | 8           |
| c6gd.large      |             | 2     | 4           |
| c6gd.medium     |             | 1     | 2           |
| c6gd.xlarge     |             | 4     | 8           |
| c6gn.large      |             | 2     | 4           |
| c6gn.medium     |             | 1     | 2           |
| c6gn.xlarge     |             | 4     | 8           |
| c6i.large       |             | 2     | 4           |
| c6i.xlarge      |             | 4     | 8           |
| c6id.large      |             | 2     | 4           |
| c6id.xlarge     |             | 4     | 8           |
| c6in.large      |             | 2     | 4           |
| c6in.xlarge     |             | 4     | 8           |
| c7a.large       |             | 2     | 4           |
| c7a.medium      |             | 1     | 2           |
| c7a.xlarge      |             | 4     | 8           |
| c7g.large       |             | 2     | 4           |
| c7g.medium      |             | 1     | 2           |
| c7g.xlarge      |             | 4     | 8           |
| c7gd.large      |             | 2     | 4           |
| c7gd.medium     |             | 1     | 2           |
| c7gd.xlarge     |             | 4     | 8           |
| c7gn.large      |             | 2     | 4           |
| c7gn.medium     |             | 1     | 2           |
| c7gn.xlarge     |             | 4     | 8           |
| c7i.large       |             | 2     | 4           |
| c7i.xlarge      |             | 4     | 8           |
| d3en.xlarge     |             | 4     | 16          |
| im4gn.large     |             | 2     | 8           |
| im4gn.xlarge    |             | 4     | 16          |
| m1.large        |             | 2     | 8           |
| m1.medium       |             | 1     | 4           |
| m1.small        |             | 1     | 2           |
| m1.xlarge       |             | 4     | 15          |
| m3.large        |             | 2     | 8           |
| m3.medium       |             | 1     | 4           |
| m3.xlarge       |             | 4     | 15          |
| m4.large        |             | 2     | 8           |
| m4.xlarge       |             | 4     | 16          |
| m5.large        |             | 2     | 8           |
| m5.xlarge       |             | 4     | 16          |
| m5a.large       |             | 2     | 8           |
| m5a.xlarge      |             | 4     | 16          |
| m5ad.large      |             | 2     | 8           |
| m5ad.xlarge     |             | 4     | 16          |
| m5d.large       |             | 2     | 8           |
| m5d.xlarge      |             | 4     | 16          |
| m5dn.large      |             | 2     | 8           |
| m5dn.xlarge     |             | 4     | 16          |
| m5n.large       |             | 2     | 8           |
| m5n.xlarge      |             | 4     | 16          |
| m5zn.large      |             | 2     | 8           |
| m5zn.xlarge     |             | 4     | 16          |
| m6a.large       |             | 2     | 8           |
| m6a.xlarge      |             | 4     | 16          |
| m6g.large       |             | 2     | 8           |
| m6g.medium      |             | 1     | 4           |
| m6g.xlarge      |             | 4     | 16          |
| m6gd.large      |             | 2     | 8           |
| m6gd.medium     |             | 1     | 4           |
| m6gd.xlarge     |             | 4     | 16          |
| m6i.large       |             | 2     | 8           |
