For Postgres:

```
CREATE TABLE prefix_paste (
    dataid CHAR(16) NOT NULL,
    data TEXT,
    postdate INT,
    expiredate INT,
    opendiscussion INT,
    burnafterreading INT,
    meta TEXT,
    attachment TEXT,
    attachmentname TEXT,
    PRIMARY KEY (dataid)
);

CREATE TABLE prefix_comment (
    dataid CHAR(16),
    pasteid CHAR(16),
    parentid CHAR(16),
    data TEXT,
    nickname TEXT,
    vizhash TEXT,
    postdate INT,
    PRIMARY KEY (dataid)
);
CREATE INDEX parent ON prefix_comment(pasteid);

CREATE TABLE prefix_config (
    id CHAR(16) NOT NULL, value TEXT, PRIMARY KEY (id)
);
INSERT INTO prefix_config VALUES('VERSION', '1.3.1');
```