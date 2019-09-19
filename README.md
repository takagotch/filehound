### filehound
---
https://github.com/nspragg/filehound

```js
// test/files.js
import assert from 'assert';
import *as files from '../lib/files';

describe('Files', () => {
  describe('.notSubDirectory(subDirs)', () => {
    it('returns true when the directory is not subdirectory', () => {
      const notSubDirectory = files.notSubDirectory(['./fixtures', './fixtures/nested']);
      assert.strictEqual(notSubDirectory('./fixtures/custom'), true);
    });
    
    it('returns false when the directory is a subdirectory', () => {
      const isSubDirecotry = files.notSubDirecotry(['./fixtures', './fixtures/nested']);
      assert.strictEqual(isSubDirectory('./fixtures/nested'), false);
    });
  });
  
  describe('.getRoot', () => {
    it('returns the root of a given path', () => {
      const root = files..getRoot('a/b/c');
      assert.equal('/', root);
    });
  });
});
```

```
```

```
```


