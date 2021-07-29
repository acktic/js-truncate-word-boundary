# js-truncate-word-boundary
Example


          let trun =
            truncate(
              complete,
              number,
              true
            );


          let truncate = function (
            i,
            n,
            useWordBoundary
          ) {
            if (
              i.length <= n
            )
              return i;
            let subString = i.substr(0, n - 1);
            return (
              (useWordBoundary
                ? subString.substr(0, subString.lastIndexOf(` `))
                : subString)
            );
          };
