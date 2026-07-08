/* @ds-bundle: {"format":3,"namespace":"BREATHEPelvicTherapyDesignSystem_fb465e","components":[{"name":"Badge","sourcePath":"components/core/Badge.jsx"},{"name":"Button","sourcePath":"components/core/Button.jsx"},{"name":"Card","sourcePath":"components/core/Card.jsx"},{"name":"Stat","sourcePath":"components/feedback/Stat.jsx"},{"name":"Input","sourcePath":"components/forms/Input.jsx"},{"name":"Textarea","sourcePath":"components/forms/Textarea.jsx"},{"name":"EyebrowHeading","sourcePath":"components/layout/EyebrowHeading.jsx"}],"sourceHashes":{"components/core/Badge.jsx":"4f49d98cf894","components/core/Button.jsx":"625b5cad0ba6","components/core/Card.jsx":"465b42affce3","components/feedback/Stat.jsx":"1bcfb17e5276","components/forms/Input.jsx":"f0e37a37ae1a","components/forms/Textarea.jsx":"d17f50dc026f","components/layout/EyebrowHeading.jsx":"8310426979a6","ui_kits/website/CTABand.jsx":"c0a2b9de0fd5","ui_kits/website/Footer.jsx":"d89113af5f02","ui_kits/website/Hero.jsx":"427d40817114","ui_kits/website/Nav.jsx":"cca09bf54e56","ui_kits/website/Services.jsx":"442d4dabbad2","ui_kits/website/Testimonial.jsx":"3bbd61206a6b"},"inlinedExternals":[],"unexposedExports":[]} */

(() => {

const __ds_ns = (window.BREATHEPelvicTherapyDesignSystem_fb465e = window.BREATHEPelvicTherapyDesignSystem_fb465e || {});

const __ds_scope = {};

(__ds_ns.__errors = __ds_ns.__errors || []);

// components/core/Badge.jsx
try { (() => {
function _extends() { return _extends = Object.assign ? Object.assign.bind() : function (n) { for (var e = 1; e < arguments.length; e++) { var t = arguments[e]; for (var r in t) ({}).hasOwnProperty.call(t, r) && (n[r] = t[r]); } return n; }, _extends.apply(null, arguments); }
const tones = {
  sage: {
    background: "var(--color-sage-mist)",
    color: "var(--color-sage-deep)"
  },
  gold: {
    background: "var(--color-gold-soft)",
    color: "var(--color-gold-deep)"
  },
  green: {
    background: "rgba(20,122,62,0.12)",
    color: "var(--color-forest-green-deep)"
  },
  blue: {
    background: "rgba(45,90,133,0.12)",
    color: "var(--color-slate-blue-deep)"
  },
  neutral: {
    background: "var(--color-sand)",
    color: "var(--color-ink-soft)"
  }
};
function Badge({
  tone = "sage",
  children,
  style,
  ...rest
}) {
  return /*#__PURE__*/React.createElement("span", _extends({
    style: {
      display: "inline-flex",
      alignItems: "center",
      fontFamily: "var(--font-body)",
      fontSize: "13px",
      fontWeight: 600,
      letterSpacing: "0.02em",
      padding: "5px 12px",
      borderRadius: "var(--radius-pill)",
      lineHeight: 1.3,
      ...tones[tone],
      ...style
    }
  }, rest), children);
}
Object.assign(__ds_scope, { Badge });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/core/Badge.jsx", error: String((e && e.message) || e) }); }

// components/core/Button.jsx
try { (() => {
function _extends() { return _extends = Object.assign ? Object.assign.bind() : function (n) { for (var e = 1; e < arguments.length; e++) { var t = arguments[e]; for (var r in t) ({}).hasOwnProperty.call(t, r) && (n[r] = t[r]); } return n; }, _extends.apply(null, arguments); }
const sizes = {
  sm: {
    padding: "10px 18px",
    fontSize: "15px"
  },
  md: {
    padding: "14px 28px",
    fontSize: "17px"
  },
  lg: {
    padding: "17px 36px",
    fontSize: "18px"
  }
};
const base = {
  fontFamily: "var(--font-body)",
  fontWeight: 600,
  letterSpacing: "0.02em",
  borderRadius: "var(--radius-md)",
  border: "1.5px solid transparent",
  cursor: "pointer",
  display: "inline-flex",
  alignItems: "center",
  justifyContent: "center",
  gap: "8px",
  transition: "all 0.2s ease",
  textDecoration: "none",
  lineHeight: 1.2
};
const variants = {
  primary: {
    background: "var(--color-gold)",
    color: "var(--color-ink)"
  },
  secondary: {
    background: "var(--color-forest-green)",
    color: "var(--color-white)"
  },
  outline: {
    background: "transparent",
    color: "var(--color-forest-green)",
    borderColor: "var(--color-forest-green)"
  },
  ghost: {
    background: "transparent",
    color: "var(--color-forest-green)"
  }
};
const hovers = {
  primary: {
    background: "var(--color-gold-deep)"
  },
  secondary: {
    background: "var(--color-forest-green-deep)"
  },
  outline: {
    background: "var(--color-sage-mist)"
  },
  ghost: {
    textDecoration: "underline"
  }
};
function Button({
  variant = "primary",
  size = "md",
  disabled = false,
  href,
  children,
  style,
  ...rest
}) {
  const [hover, setHover] = React.useState(false);
  const composed = {
    ...base,
    ...sizes[size],
    ...variants[variant],
    ...(hover && !disabled ? hovers[variant] : null),
    ...(disabled ? {
      opacity: 0.5,
      cursor: "not-allowed"
    } : null),
    ...style
  };
  const Tag = href ? "a" : "button";
  return /*#__PURE__*/React.createElement(Tag, _extends({
    href: href,
    style: composed,
    disabled: href ? undefined : disabled,
    onMouseEnter: () => setHover(true),
    onMouseLeave: () => setHover(false)
  }, rest), children);
}
Object.assign(__ds_scope, { Button });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/core/Button.jsx", error: String((e && e.message) || e) }); }

// components/core/Card.jsx
try { (() => {
function _extends() { return _extends = Object.assign ? Object.assign.bind() : function (n) { for (var e = 1; e < arguments.length; e++) { var t = arguments[e]; for (var r in t) ({}).hasOwnProperty.call(t, r) && (n[r] = t[r]); } return n; }, _extends.apply(null, arguments); }
function Card({
  as: Tag = "div",
  surface = "white",
  hover = false,
  children,
  style,
  ...rest
}) {
  const [h, setH] = React.useState(false);
  const bg = surface === "sand" ? "var(--color-sand)" : "var(--color-white)";
  return /*#__PURE__*/React.createElement(Tag, _extends({
    onMouseEnter: () => hover && setH(true),
    onMouseLeave: () => hover && setH(false),
    style: {
      background: bg,
      border: "1px solid var(--color-sand-deep)",
      borderRadius: "var(--radius-lg)",
      padding: "var(--space-6)",
      transition: "all 0.2s ease",
      ...(h ? {
        transform: "translateY(-4px)",
        boxShadow: "var(--shadow-lg)",
        borderColor: "transparent"
      } : null),
      ...style
    }
  }, rest), children);
}
Object.assign(__ds_scope, { Card });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/core/Card.jsx", error: String((e && e.message) || e) }); }

// components/feedback/Stat.jsx
try { (() => {
function Stat({
  value,
  label,
  align = "left",
  style
}) {
  return /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      flexDirection: "column",
      gap: "4px",
      textAlign: align,
      fontFamily: "var(--font-body)",
      ...style
    }
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      fontFamily: "var(--font-display)",
      fontWeight: 500,
      fontSize: "48px",
      lineHeight: 1,
      color: "var(--color-forest-green)",
      fontVariantNumeric: "tabular-nums"
    }
  }, value), /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: "15px",
      color: "var(--color-ink-soft)"
    }
  }, label));
}
Object.assign(__ds_scope, { Stat });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/feedback/Stat.jsx", error: String((e && e.message) || e) }); }

// components/forms/Input.jsx
try { (() => {
function _extends() { return _extends = Object.assign ? Object.assign.bind() : function (n) { for (var e = 1; e < arguments.length; e++) { var t = arguments[e]; for (var r in t) ({}).hasOwnProperty.call(t, r) && (n[r] = t[r]); } return n; }, _extends.apply(null, arguments); }
function Input({
  label,
  hint,
  error,
  id,
  style,
  ...rest
}) {
  const [focus, setFocus] = React.useState(false);
  const inputId = id || (label ? label.toLowerCase().replace(/\s+/g, "-") : undefined);
  return /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      flexDirection: "column",
      gap: "6px",
      fontFamily: "var(--font-body)"
    }
  }, label && /*#__PURE__*/React.createElement("label", {
    htmlFor: inputId,
    style: {
      fontSize: "13px",
      fontWeight: 600,
      color: "var(--color-ink-soft)"
    }
  }, label), /*#__PURE__*/React.createElement("input", _extends({
    id: inputId,
    onFocus: () => setFocus(true),
    onBlur: () => setFocus(false),
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "16px",
      color: "var(--color-ink)",
      background: "var(--color-white)",
      border: `1px solid ${error ? "var(--color-error)" : focus ? "var(--color-forest-green)" : "var(--color-stone)"}`,
      borderRadius: "var(--radius-sm)",
      padding: "12px 16px",
      outline: "none",
      transition: "all 0.2s ease",
      boxShadow: focus ? "0 0 0 3px rgba(20,122,62,0.15)" : "none",
      ...style
    }
  }, rest)), (hint || error) && /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: "12px",
      color: error ? "var(--color-error)" : "var(--color-ink-muted)"
    }
  }, error || hint));
}
Object.assign(__ds_scope, { Input });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/forms/Input.jsx", error: String((e && e.message) || e) }); }

// components/forms/Textarea.jsx
try { (() => {
function _extends() { return _extends = Object.assign ? Object.assign.bind() : function (n) { for (var e = 1; e < arguments.length; e++) { var t = arguments[e]; for (var r in t) ({}).hasOwnProperty.call(t, r) && (n[r] = t[r]); } return n; }, _extends.apply(null, arguments); }
function Textarea({
  label,
  hint,
  id,
  rows = 4,
  style,
  ...rest
}) {
  const [focus, setFocus] = React.useState(false);
  const inputId = id || (label ? label.toLowerCase().replace(/\s+/g, "-") : undefined);
  return /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      flexDirection: "column",
      gap: "6px",
      fontFamily: "var(--font-body)"
    }
  }, label && /*#__PURE__*/React.createElement("label", {
    htmlFor: inputId,
    style: {
      fontSize: "13px",
      fontWeight: 600,
      color: "var(--color-ink-soft)"
    }
  }, label), /*#__PURE__*/React.createElement("textarea", _extends({
    id: inputId,
    rows: rows,
    onFocus: () => setFocus(true),
    onBlur: () => setFocus(false),
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "16px",
      lineHeight: 1.6,
      color: "var(--color-ink)",
      background: "var(--color-white)",
      border: `1px solid ${focus ? "var(--color-forest-green)" : "var(--color-stone)"}`,
      borderRadius: "var(--radius-sm)",
      padding: "12px 16px",
      outline: "none",
      resize: "vertical",
      transition: "all 0.2s ease",
      boxShadow: focus ? "0 0 0 3px rgba(20,122,62,0.15)" : "none",
      ...style
    }
  }, rest)), hint && /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: "12px",
      color: "var(--color-ink-muted)"
    }
  }, hint));
}
Object.assign(__ds_scope, { Textarea });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/forms/Textarea.jsx", error: String((e && e.message) || e) }); }

// components/layout/EyebrowHeading.jsx
try { (() => {
const aligns = {
  left: "flex-start",
  center: "center"
};
const tones = {
  sage: "var(--color-sage-deep)",
  gold: "var(--color-gold-deep)"
};
function EyebrowHeading({
  eyebrow,
  title,
  lead,
  align = "left",
  eyebrowTone = "sage",
  rule = false,
  level = 2,
  style
}) {
  const Heading = `h${level}`;
  return /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      flexDirection: "column",
      alignItems: aligns[align],
      textAlign: align,
      gap: "14px",
      fontFamily: "var(--font-body)",
      ...style
    }
  }, eyebrow && /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: "13px",
      fontWeight: 600,
      letterSpacing: "0.12em",
      textTransform: "uppercase",
      color: tones[eyebrowTone]
    }
  }, eyebrow), /*#__PURE__*/React.createElement(Heading, {
    style: {
      fontFamily: "var(--font-display)",
      fontWeight: 500,
      fontSize: "clamp(28px, 4vw, 36px)",
      lineHeight: 1.1,
      color: "var(--color-ink)",
      margin: 0,
      maxWidth: "18ch"
    }
  }, title), lead && /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: "19px",
      lineHeight: 1.6,
      color: "var(--color-ink-soft)",
      margin: 0,
      maxWidth: "56ch"
    }
  }, lead), rule && /*#__PURE__*/React.createElement("span", {
    style: {
      width: "40px",
      height: "2px",
      background: "var(--color-gold)",
      marginTop: "4px"
    }
  }));
}
Object.assign(__ds_scope, { EyebrowHeading });
})(); } catch (e) { __ds_ns.__errors.push({ path: "components/layout/EyebrowHeading.jsx", error: String((e && e.message) || e) }); }

// ui_kits/website/CTABand.jsx
try { (() => {
// CTA band — full-bleed forest-green anchor section with gold primary button.
function CTABand() {
  const {
    Button
  } = window.BREATHEPelvicTherapyDesignSystem_fb465e;
  return /*#__PURE__*/React.createElement("section", {
    style: {
      background: "var(--color-forest-green-deep)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-narrow)",
      margin: "0 auto",
      padding: "96px 48px",
      textAlign: "center"
    }
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: "13px",
      fontWeight: 600,
      letterSpacing: "0.12em",
      textTransform: "uppercase",
      color: "var(--color-gold-soft)"
    }
  }, "Take the first step"), /*#__PURE__*/React.createElement("h2", {
    style: {
      fontFamily: "var(--font-display)",
      fontWeight: 500,
      fontSize: "44px",
      lineHeight: 1.1,
      color: "var(--color-white)",
      margin: "16px 0 18px"
    }
  }, "Strength starts with your breath"), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: "19px",
      lineHeight: 1.6,
      color: "rgba(251,248,242,0.85)",
      margin: "0 auto 32px",
      maxWidth: "48ch"
    }
  }, "Book a free, pressure-free discovery call and let's talk about where you want to feel strong again."), /*#__PURE__*/React.createElement(Button, {
    variant: "primary",
    size: "lg"
  }, "Book a free discovery call")));
}
window.CTABand = CTABand;
})(); } catch (e) { __ds_ns.__errors.push({ path: "ui_kits/website/CTABand.jsx", error: String((e && e.message) || e) }); }

// ui_kits/website/Footer.jsx
try { (() => {
// Footer — dark green, logo, link columns, fine print.
function Footer() {
  const cols = [{
    h: "Services",
    links: ["Pregnancy care", "Postpartum recovery", "Pelvic pain", "Strength & fitness"]
  }, {
    h: "Practice",
    links: ["Our approach", "About us", "Resources", "Careers"]
  }, {
    h: "Visit",
    links: ["Book now", "Contact", "Insurance", "FAQ"]
  }];
  return /*#__PURE__*/React.createElement("footer", {
    style: {
      background: "var(--color-forest-green-deep)",
      borderTop: "1px solid rgba(255,255,255,0.12)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-max)",
      margin: "0 auto",
      padding: "72px 48px 40px",
      display: "grid",
      gridTemplateColumns: "1.4fr repeat(3, 1fr)",
      gap: "48px"
    }
  }, /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("img", {
    src: "../../assets/logo-full-light.png",
    alt: "BREATHE Pelvic Health Center",
    style: {
      height: "84px",
      marginBottom: "16px"
    }
  }), /*#__PURE__*/React.createElement("p", {
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "15px",
      lineHeight: 1.7,
      color: "rgba(251,248,242,0.7)",
      margin: 0,
      maxWidth: "32ch"
    }
  }, "Elegant, evidence-based pelvic health care. Care that meets you where you are.")), cols.map(c => /*#__PURE__*/React.createElement("div", {
    key: c.h
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "13px",
      fontWeight: 600,
      letterSpacing: "0.08em",
      textTransform: "uppercase",
      color: "var(--color-gold-soft)",
      marginBottom: "16px"
    }
  }, c.h), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      flexDirection: "column",
      gap: "10px"
    }
  }, c.links.map(l => /*#__PURE__*/React.createElement("a", {
    key: l,
    href: "#",
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "15px",
      color: "rgba(251,248,242,0.8)",
      textDecoration: "none"
    }
  }, l)))))), /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-max)",
      margin: "0 auto",
      padding: "20px 48px 40px",
      borderTop: "1px solid rgba(255,255,255,0.12)",
      display: "flex",
      justifyContent: "space-between",
      flexWrap: "wrap",
      gap: "12px",
      fontFamily: "var(--font-body)",
      fontSize: "13px",
      color: "rgba(251,248,242,0.6)"
    }
  }, /*#__PURE__*/React.createElement("span", null, "\xA9 2026 BREATHE Pelvic Health Center"), /*#__PURE__*/React.createElement("span", null, "Privacy \xB7 Terms \xB7 Accessibility")));
}
window.Footer = Footer;
})(); } catch (e) { __ds_ns.__errors.push({ path: "ui_kits/website/Footer.jsx", error: String((e && e.message) || e) }); }

// ui_kits/website/Hero.jsx
try { (() => {
// Hero — eyebrow + serif headline + lead + CTAs, asymmetric 6/5 split with arch-topped image.
function Hero() {
  const {
    Button,
    Badge
  } = window.BREATHEPelvicTherapyDesignSystem_fb465e;
  return /*#__PURE__*/React.createElement("section", {
    style: {
      background: "var(--color-cream)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-max)",
      margin: "0 auto",
      padding: "96px 48px",
      display: "grid",
      gridTemplateColumns: "1.1fr 0.9fr",
      gap: "64px",
      alignItems: "center"
    }
  }, /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: "13px",
      fontWeight: 600,
      letterSpacing: "0.12em",
      textTransform: "uppercase",
      color: "var(--color-sage-deep)"
    }
  }, "Pelvic Health Center"), /*#__PURE__*/React.createElement("h1", {
    style: {
      fontFamily: "var(--font-display)",
      fontWeight: 500,
      fontSize: "60px",
      lineHeight: 1.05,
      color: "var(--color-ink)",
      margin: "18px 0 20px",
      maxWidth: "14ch"
    }
  }, "Heal at your own pace"), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: "20px",
      lineHeight: 1.6,
      color: "var(--color-ink-soft)",
      margin: "0 0 32px",
      maxWidth: "46ch"
    }
  }, "Gentle, evidence-based pelvic floor care \u2014 for pregnancy, postpartum, and life. Your symptoms are a story, and we are here to listen."), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: "16px",
      alignItems: "center",
      flexWrap: "wrap"
    }
  }, /*#__PURE__*/React.createElement(Button, {
    variant: "primary",
    size: "lg"
  }, "Book a free discovery call"), /*#__PURE__*/React.createElement(Button, {
    variant: "ghost",
    size: "lg",
    style: {
      padding: "17px 8px"
    }
  }, "See how it works \u2192")), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: "10px",
      marginTop: "28px"
    }
  }, /*#__PURE__*/React.createElement(Badge, {
    tone: "sage"
  }, "Pregnancy"), /*#__PURE__*/React.createElement(Badge, {
    tone: "sage"
  }, "Postpartum"), /*#__PURE__*/React.createElement(Badge, {
    tone: "sage"
  }, "Core & fitness"))), /*#__PURE__*/React.createElement("div", {
    style: {
      position: "relative",
      aspectRatio: "4/5",
      borderRadius: "180px 180px var(--radius-xl) var(--radius-xl)",
      background: "linear-gradient(160deg, var(--color-sage-mist), var(--color-sage))",
      border: "1px solid var(--color-sand-deep)",
      display: "flex",
      alignItems: "flex-end",
      justifyContent: "center",
      overflow: "hidden"
    }
  }, /*#__PURE__*/React.createElement("img", {
    src: "../../assets/leaf-mark.png",
    alt: "",
    style: {
      width: "96px",
      opacity: 0.55,
      marginBottom: "40px"
    }
  }), /*#__PURE__*/React.createElement("span", {
    style: {
      position: "absolute",
      top: "16px",
      left: "16px",
      fontSize: "12px",
      color: "var(--color-ink-muted)",
      fontFamily: "var(--font-body)"
    }
  }, "[ warm lifestyle photo ]"))));
}
window.Hero = Hero;
})(); } catch (e) { __ds_ns.__errors.push({ path: "ui_kits/website/Hero.jsx", error: String((e && e.message) || e) }); }

// ui_kits/website/Nav.jsx
try { (() => {
// BREATHE marketing site — sticky top navigation.
function Nav() {
  const {
    Button
  } = window.BREATHEPelvicTherapyDesignSystem_fb465e;
  const links = ["Services", "Our approach", "About", "Resources"];
  return /*#__PURE__*/React.createElement("header", {
    style: {
      position: "sticky",
      top: 0,
      zIndex: 20,
      background: "rgba(251,248,242,0.88)",
      backdropFilter: "blur(10px)",
      borderBottom: "1px solid var(--color-sand-deep)"
    }
  }, /*#__PURE__*/React.createElement("nav", {
    style: {
      maxWidth: "var(--container-max)",
      margin: "0 auto",
      padding: "16px 48px",
      display: "flex",
      alignItems: "center",
      gap: "32px"
    }
  }, /*#__PURE__*/React.createElement("a", {
    href: "#",
    style: {
      display: "flex",
      alignItems: "center"
    }
  }, /*#__PURE__*/React.createElement("img", {
    src: "../../assets/logo-full.png",
    alt: "BREATHE Pelvic Health Center",
    style: {
      height: "52px"
    }
  })), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      gap: "28px",
      marginLeft: "16px",
      flex: 1
    }
  }, links.map(l => /*#__PURE__*/React.createElement("a", {
    key: l,
    href: "#",
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "15px",
      fontWeight: 500,
      color: "var(--color-ink)",
      textDecoration: "none"
    }
  }, l))), /*#__PURE__*/React.createElement("a", {
    href: "#",
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "15px",
      fontWeight: 500,
      color: "var(--color-ink-soft)",
      textDecoration: "none"
    }
  }, "Sign in"), /*#__PURE__*/React.createElement(Button, {
    variant: "primary",
    size: "sm"
  }, "Book now")));
}
window.Nav = Nav;
})(); } catch (e) { __ds_ns.__errors.push({ path: "ui_kits/website/Nav.jsx", error: String((e && e.message) || e) }); }

// ui_kits/website/Services.jsx
try { (() => {
// Services — 3-column card grid of service tiles (sand section for rhythm).
function Services() {
  const {
    Card,
    EyebrowHeading,
    Button
  } = window.BREATHEPelvicTherapyDesignSystem_fb465e;
  const items = [{
    icon: "baby",
    title: "Pregnancy care",
    body: "Stay strong and comfortable through every trimester with guided, gentle support."
  }, {
    icon: "heart-handshake",
    title: "Postpartum recovery",
    body: "Rebuild core and pelvic-floor strength at your own pace, with one-on-one care."
  }, {
    icon: "activity",
    title: "Bladder & bowel health",
    body: "Address leaks, urgency, and discomfort with proven, dignified treatment."
  }, {
    icon: "flower-2",
    title: "Pelvic pain relief",
    body: "Find lasting relief from pain that too often goes unspoken and untreated."
  }, {
    icon: "dumbbell",
    title: "Strength & fitness",
    body: "Return to movement you love — running, lifting, and everyday life — safely."
  }, {
    icon: "messages-square",
    title: "Discovery call",
    body: "Not sure where to start? A free, pressure-free conversation about your goals."
  }];
  return /*#__PURE__*/React.createElement("section", {
    style: {
      background: "var(--color-sand)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-max)",
      margin: "0 auto",
      padding: "112px 48px"
    }
  }, /*#__PURE__*/React.createElement(EyebrowHeading, {
    eyebrow: "What we treat",
    title: "Care for every stage of your story",
    lead: "One-on-one, never rushed. Choose a focus below or start with a free discovery call.",
    rule: true,
    style: {
      marginBottom: "56px"
    }
  }), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "grid",
      gridTemplateColumns: "repeat(3, 1fr)",
      gap: "24px"
    }
  }, items.map(it => /*#__PURE__*/React.createElement(Card, {
    key: it.title,
    hover: true
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      width: "48px",
      height: "48px",
      borderRadius: "var(--radius-md)",
      background: "var(--color-sage-mist)",
      display: "flex",
      alignItems: "center",
      justifyContent: "center",
      marginBottom: "20px"
    }
  }, /*#__PURE__*/React.createElement("i", {
    "data-lucide": it.icon,
    style: {
      color: "var(--color-forest-green)"
    }
  })), /*#__PURE__*/React.createElement("h3", {
    style: {
      fontFamily: "var(--font-display)",
      fontWeight: 500,
      fontSize: "23px",
      color: "var(--color-ink)",
      margin: "0 0 10px"
    }
  }, it.title), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: "16px",
      lineHeight: 1.7,
      color: "var(--color-ink-soft)",
      margin: "0 0 18px"
    }
  }, it.body), /*#__PURE__*/React.createElement(Button, {
    variant: "ghost",
    style: {
      padding: 0
    }
  }, "Learn more \u2192"))))));
}
window.Services = Services;
})(); } catch (e) { __ds_ns.__errors.push({ path: "ui_kits/website/Services.jsx", error: String((e && e.message) || e) }); }

// ui_kits/website/Testimonial.jsx
try { (() => {
// Testimonial — centered serif quote with large quotation flourish + stats band.
function Testimonial() {
  const {
    Stat
  } = window.BREATHEPelvicTherapyDesignSystem_fb465e;
  return /*#__PURE__*/React.createElement("section", {
    style: {
      background: "var(--color-cream)"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-narrow)",
      margin: "0 auto",
      padding: "112px 48px",
      textAlign: "center"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      fontFamily: "var(--font-display)",
      fontSize: "80px",
      lineHeight: 0.6,
      color: "var(--color-gold-soft)",
      marginBottom: "8px"
    }
  }, "\u201C"), /*#__PURE__*/React.createElement("blockquote", {
    style: {
      fontFamily: "var(--font-display)",
      fontWeight: 500,
      fontSize: "32px",
      lineHeight: 1.35,
      color: "var(--color-ink)",
      margin: "0 0 28px"
    }
  }, "For the first time, I felt heard. BREATHE gave me back the confidence I thought I had lost after my second pregnancy."), /*#__PURE__*/React.createElement("div", {
    style: {
      fontFamily: "var(--font-body)",
      fontSize: "14px",
      fontWeight: 600,
      letterSpacing: "0.02em",
      color: "var(--color-ink-soft)"
    }
  }, "MAYA R. \xB7 Postpartum recovery")), /*#__PURE__*/React.createElement("div", {
    style: {
      maxWidth: "var(--container-max)",
      margin: "0 auto",
      padding: "0 48px 112px"
    }
  }, /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-around",
      gap: "32px",
      flexWrap: "wrap",
      background: "var(--color-sage-mist)",
      borderRadius: "var(--radius-xl)",
      padding: "48px 32px"
    }
  }, /*#__PURE__*/React.createElement(Stat, {
    value: "92%",
    label: "report symptom relief",
    align: "center"
  }), /*#__PURE__*/React.createElement(Stat, {
    value: "5k+",
    label: "sessions delivered",
    align: "center"
  }), /*#__PURE__*/React.createElement(Stat, {
    value: "4.9",
    label: "average client rating",
    align: "center"
  }), /*#__PURE__*/React.createElement(Stat, {
    value: "1:1",
    label: "always one-on-one",
    align: "center"
  }))));
}
window.Testimonial = Testimonial;
})(); } catch (e) { __ds_ns.__errors.push({ path: "ui_kits/website/Testimonial.jsx", error: String((e && e.message) || e) }); }

__ds_ns.Badge = __ds_scope.Badge;

__ds_ns.Button = __ds_scope.Button;

__ds_ns.Card = __ds_scope.Card;

__ds_ns.Stat = __ds_scope.Stat;

__ds_ns.Input = __ds_scope.Input;

__ds_ns.Textarea = __ds_scope.Textarea;

__ds_ns.EyebrowHeading = __ds_scope.EyebrowHeading;

})();
