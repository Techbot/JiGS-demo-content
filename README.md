# JiGS Demo Content

Add the UUID in `jigs_demo_content.info.yml`
```
default_content:
  node:

  menu_link_content:

  block_content:

  taxonomy_term:

```
Then run `drush dcem jigs_demo_content`

To get UUIDs:
```bash
drush sqlq "select * from media"
drush sqlq "select * from file_managed"
drush sqlq "select * from taxonomy_term_data"
drush sqlq "select * from block_content"
drush sqlq "select * from menu_link_content"
```
 See https://www.drupal.org/docs/contributed-modules/default-content-for-d8/defining-default-content

```
drush sqlq "select * from node"
1	1	city	f6fc8bde-c606-419f-b1e3-500544cd15dd	en
2	2	game	ff690241-146d-4a2c-b107-28529f746008	en
3	3	map_grid	33016d96-c1b9-4362-9be9-f79f1de0a53a	en
4	4	mob	0565b0d9-225e-42ac-bf53-046d01d3b386	en
5	16	weapon	ba9e4061-a213-40e0-8f17-bdffa4eda6ac	en
6	6	skill	6920c31d-174f-4865-8185-a50d29674095	en
7	15	npc	451a4996-627f-4cb7-b1e9-07c72889ebb3	en
8	13	items	6415e584-2814-4681-9c88-2dae0862403e	en
9	9	component	dd710392-75ca-46b5-a49b-9d639356cabc	en
10	11	faction	a3a432c4-7a7e-4c69-8087-a545c64db8c5	en

drush sqlq "select * from taxonomy_term_data"
1	1	tilemaps	d4b0100b-022b-487f-90b1-9e544769e30b	en
2	2	tilemaps	2e00fc0b-9c49-4c4b-b8c8-e7ddf3b004ff	en
3	3	faction_type	2b611a76-32c5-4b17-abf5-6b87aaf51c29	en
4	4	ammo_type	7d3fd514-cc49-4aaa-8133-e27a3e91c9bd	en
6	6	item_type	6d593e8c-e411-4e80-a7fb-d3a2eee8c0c0	en
7	7	mob_type	24e5da17-a438-47a0-9769-85167b95f77c	en
8	8	modifer_type	12286216-be6f-4f19-ab83-fd320671ef8e	en
9	9	occupation	47b24664-61dd-4d68-a0d8-10035b780614	en
10	10	race	d8dff635-2144-4cb3-acd0-dc9c9fef09a1	en
11	11	item_type	d76fcd85-64d7-4ee8-a0f6-ffdb91ccc3c4	en
12	12	concerns	849befe3-5fcb-42ea-b049-ae88a5e8acda	en

drush sqlq "select * from profile"
1	1	player	64c1ae38-32ed-4bed-806e-1b9160ccc1f8	1	1	1	a:0:{}	1706557348	1706733783
2	2	faction	25537bc0-72ac-4aa8-a9c2-d34fd7f8d03e	1	2	1	a:0:{}	1706645385	1706733859
3	3	player	4bd054f2-d7b9-4766-a64d-eeac6bd0ccd6	1	2	1	a:0:{}	1706733932	1706733959

drush sqlq "select * from users"
1	787c8646-b3ef-4f3a-86a4-250d0217b725	en
2	c01eda2e-7e6f-467b-9cab-fd286e2b43fb	en


```
