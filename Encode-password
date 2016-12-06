  encodePW = function(username, password) {
    var i, md5, sha1, _i;
    md5 = crypto.createHash('md5');
    md5.update(password);
    password = username + md5.digest('hex');
    for (i = _i = 0; _i < 1000; i = ++_i) {
      sha1 = crypto.createHash('sha1');
      sha1.update(password);
      password = sha1.digest('hex');
    }
    return password;
  };
