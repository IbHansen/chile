# ModelFlow models for Chile

This book collects ModelFlow versions of Chilean macro-fiscal and pension models. The first is
the deterministic macro-fiscal / pension model, ported from the Stata do-file
`model_macrofiscal_deterministic.do`.

- **[Five scenarios](chile_scenarios.ipynb).** The model is loaded and five exogenous variables
  are shocked one at a time: the VAT rate, pension benefits, the health-spending elasticity,
  female participation and the copper price.
- **[The scenarios with sliders](chile_scenario_widget.ipynb).** The same five shocks as sliders
  in a widget, to run, name and compare your own scenarios. The chapter runs in your browser:
  press the power button at the top of the page. The other chapters are meant to be read.
- **[Loading the macro-fiscal model](chile_macrofiscal_deterministic.ipynb).** How the model gets
  into ModelFlow: it is written block by block with `%%Makemymodel`, three equations are
  estimated in place, and the solution 2025-2070 is compared with Stata's to show that the model
  is loaded correctly. The model and its data are saved in `data/chilepens.pcim`, which the
  scenarios use.
- **[Model documentation](model_documentation.md).** The equations block by block with their
  explanations and the estimation results. The loading notebook generates this chapter from the
  model itself, so it can serve as the paper presenting the model, always in sync with the model.
- **[Testing the scenario widget](chile_widget_test.ipynb).** Runs the five scenarios through the
  slider widget and checks that they equal the same shocks made with `upd`.

More models will follow.
