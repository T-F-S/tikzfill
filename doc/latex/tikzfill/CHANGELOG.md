# Changelog
All notable changes to this project will be documented in this file.

The format is based on
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to
[Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
### Changed
### Deprecated
### Removed
### Fixed
### Security



## [1.2.0] - 2026-04-23

### Added
- Library `tikzfill.geomarray`:
    TikZ Options:
        `fill gea Niederhatzkofen`, `fill gea Marktstauden`, 
        `fill gea Alpersdorf`, `fill gea Scheckenhofen`, `fill gea Edenland`,
        `fill gea Klosterholz`, `fill gea Baumgarten`, `fill gea Ostergaden`,
        `fill gea Eggerach`, `fill gea Schwarzberg`
    Customization Options:
        `xflip`, `xflip even`, `xflip odd`, `yflip`, `yflip even`, `yflip odd`,
        `style base`, `style 10`, `style 11`, `style 12`, `style 13`, `style 14`,
        `prime color 1`, `prime color 2`, `ratio`, `debug node`,
        `draw-if-row-col`, `draw-if-not-row-col`,
        `draw-if-row`, `draw-if-not-row`, `draw-if-even-row`, `draw-if-odd-row`,
        `draw-if-col`, `draw-if-not-col`, `draw-if-even-col`, `draw-if-odd-col`,
        `draw-if-random`
    Read-only macros:
        `\l_tikzfill_gea_prime_col_i_tl`, `\l_tikzfill_gea_prime_col_ii_tl`,
        `\l_tikzfill_gea_ratio_tl`

### Changed
- Title page reworked

### Fixed
- Template `Weihmichl`



## [1.1.0] - 2026-03-26

### Added
- New library `tikzfill.geomarray` for drawing small pictures arranged on a grid.
    TikZ Options:
        `fill geomarray`, `fill gea Altdorf`, `fill gea Loeschenbrand`,
        `fill gea Ganslberg`, `fill gea Essenbach`, `fill gea Mirskofen`,
        `fill gea Bruckberg`, `fill gea Bachhorn`, `fill gea Furth`,
        `fill gea Schatzhofen`, `fill gea Pfettrach`, `fill gea Kolmhub`,
        `fill gea Weihmichl`, `fill gea Ergolding`, `fill gea Hascherkeller`,
        `fill gea Unterglaim`, `fill gea Grandsberg`, `fill gea Kottingrohr`,
        `fill gea Hohenthann`, `fill gea Bibelsbach`, `fill gea Roseneck`,
        `fill gea Altenkofen`, `fill gea Irlmuehle`, `fill gea Gammelsdorf`,
        `fill gea Traich`, `fill gea Winbuerg`,`fill gea Kreuzholzen`,
        `fill gea Grafenhaun`
    Customization Options:
        `triangular`, `xstep`, `ystep`, `ystep equidistance`, `ystep equidistance*`,
        `step`, `step half`, `step double`, `step equi`, `step equi*`,
        `step equi half`, `step equi* half`, `step equi double`, `step equi* double`,
        `angle`, `scale`, `scale linear`, `scale fixed`, `debug text`,
        `init`, `init<`, `init>`, `init-row`, `init-row<`, `init-row>`,
        `init-item`, `init-item<`, `init-item>`, `draw-item`, `draw-item<`, `draw-item>`,        
        `node`, `node>`, `node<`, `text`, `text<`, `text>`, `freeze-row`,
        `style 1`, `style 2`, `style 3`, `style 4`, `style 5`, `style 6`,
        `style 7`, `style 8`, `style 9`
    Read-only macros:
        `\l_tikzfill_gea_xstep_dim`, `\l_tikzfill_gea_ystep_dim`,
        `\l_tikzfill_gea_frac_fp`, `\l_tikzfill_gea_scale_fp`,
        `\l_tikzfill_gea_rows_int`, `\l_tikzfill_gea_cols_int`,
        `\l_tikzfill_gea_row_tl`, `\l_tikzfill_gea_col_tl`
    Macros:    
        `\TFRowColorLet`, `\TFRowColorLetSeq`,`\TFDefineRandomColor`,

### Changed
- `CHANGES.md` renamed to `CHANGELOG.md` following https://keepachangelog.com/en/1.1.0/
- `tikzfill-doc.sty` renamed to `tikzfill.doc.sty`
- Scratch variables like `\l_tmpa_fp` replaced by package variables
- New cover with `fill geomarray`

### Removed
- `tikzfill-common.sty` (not needed any longer)
- Check for expl3 existence

### Fixed
- Documentation typos fixed (issue #3)
- Documentation structural multiple label warnings fixed
- `tikzlibraryfill.rhombus.code.tex` had wrong version information
- Code style improved with explcheck 



## [1.0.1] - 2023-08-08

### Added
- Input of `expl3-generic` where `ExplSyntaxOn` is not defined (issue #1)

### Removed
- Library `fill.image`: Unused code fragments

### Fixed
- Spelling of LaTeX etc. inside the documentation (issue #1)
- Package loading implementation changed to LaTeX2e by adapting a TikZ macro
    to fix package loading problems (issue #2)



## [1.0.0] - 2022-07-20

### Added
- Initial public release
